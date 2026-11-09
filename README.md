# Runcress 1.0 TEST
Native Android Lohkous region-run puzzle. Android 8+ (min26), target35. Package com.gg007.runcress. Twelve original unique boards on a compact 4x3 grid.

## Rules
Lohkous on a 4x3 grid. Fence all cells into side-connected regions, each containing exactly one clue cell. A clue lists ALL distinct lengths of maximal horizontal and vertical cell runs within its region. Every listed length must occur at least once; repeats are allowed. A run counts cells, not border edges or a bounding box. No extra internal fences. Tap thin cell borders to add/remove fences. Undo/reset and next/levels; saved palette and optional current-region letters. Known Lohkous adaptation.

## Download and status
https://mega.co.nz/#!MBVFHS6a!3FrH02h8TbNugNc_NsG_e1PrIntUNBCgdjKx9ksHofg
APK SHA256 2455fa28baf2574b3d06fe940d2feefc76e6ac0dc87fd711600d5169f1f14940; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
A portable seed-721110 generator enumerates all connected subsets of the twelve cells and their run-length sets, then creates original clue layouts and counts exact-cover partitions. Twelve different boards each have one legal partition. An independent oracle uses union-find and complete row/column scans, while production uses flood regions and run-start scanning. All 1,572,864 fence-mask comparisons agree. Canonical borders reject internal stray fences. Bounds, toggle, undo/reset and solved lock pass. Actual drawing-adapter fence taps solve all twelve and check undo/replay, next, levels, menu, privacy and saved palette/region letters. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 203 live studio descriptions and current 803-entry web registry using functional terms. No Lohkous, region-run-length or horizontal/vertical-run text matches in the web registry. Poolcress constrains whole straight segments of a drawn loop in predefined rooms. Runcress instead partitions every cell into arbitrary connected regions and constrains their cell-run lengths, with exactly one clue per region and no loop. Sumhaven and Mosaicmeadow require rectangles and width-plus-height or area clues, not run-length sets. Known Lohkous adaptation; original generated layouts, code and visuals. No copied layouts/code/art or global invention/history claim. Six fetched sources include the original creator rule image, independent setters, an encyclopedia and puzzle clubs. Variant-only wildcard/ice/Nikoji rules are not used.
Rules https://www.hempuli.com/blog/index.php?rule=id&ruleid=535 ; independent rules https://brokensign.com/puzzle/2022/11/24/lohkous.html .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/runcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.runcress.RunBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Runcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, region letters and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 204-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/43e51zj43cmd-runcress-source-archive . Repository https://github.com/iLanis-agent/runcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
