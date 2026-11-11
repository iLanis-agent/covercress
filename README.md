# Covercress 1.0 TEST
Native Android minimum-cost set cover puzzle. Android 8+ min26/target35. Package com.gg007.covercress.

## Rules
Known weighted-set-cover adaptation. Seven bundles each contain some letters from A-H and have a printed whole-bundle cost. Tap bundle rows to choose or remove them. Every letter A-H must appear in at least one chosen bundle. Overlaps are allowed and do not add a penalty: pay each selected bundle cost once. Minimize total cost and press CHECK COVER. This is not exact cover; duplicate coverage is valid. Gold top letters are covered, gray letters are missing. Twelve original seven-bundle instances with one optimum each, using 3-4 bundles and some duplicate coverage in every optimum. Undo/reset, GG007 menu/site/privacy and saved palette/optional bundle numbers. Tap the title or Android Back for menu.

## Download and status
https://mega.co.nz/#!pNk0kYqQ!ncjEndAMFlZJeTYEt64bC2EcGbuO86YcN5gjhk2FgUU
APK 20974 bytes; SHA256 cfd8d71a36e30f70d5f25d52e4241ef30ea2fd325c8ec23e233e95ebfa11ceb1. Original certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions, original GG007 icon unchanged. Anonymous downloaded bytes match.

## Checks
Seed 1041111 produces twelve distinct seven-bundle instances over eight symbols. All 128 subsets per level,1536 total, independently compare element membership counts and summed cost with production bitmask union and minimum-cost coverage dynamic programming. Another 10752 bundle-toggle/undo transitions verify restoration;1000 random seven-bundle cases compare DP against exhaustive covers. Explicit missing-symbol, overpriced-cover, valid-overlap, empty-set, invalid mask/bundle bounds, invalid bundle data and reset tests pass. All twelve actual drawing-adapter bundle/CHECK optimum tap-solves, empty/all-bundle rejections, solved locks, actual NEXT, undo/reset/levels/title-menu/privacy/saved palette-labels pass. Twenty drawing previews inspected, not phone screenshots. Phone runtime, performance, browser handoff QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
All 235 prior studio descriptions reviewed. The 803 legacy registry is byte-identical to its reviewed baseline; set-cover/covering/subset/budget/minimum-cover scan found no matching minimum-cost set-union mechanic. Covercress minimizes cost subject to union covering every required symbol, with overlap allowed. Slotcress maximizes reward subject to pairwise time incompatibility; Weightwake matches separate weighted row/column sums; Willowcourt partitions cells with exactly one clue per rectangle. Those constraints do not implement overlapping set union and coverage DP. Known weighted set cover, not globally new. Original seeded bundle memberships/costs, native implementation and coverage matrix illustration. Six university, library-documentation and encyclopedia sources used for definition and at-least-one convention. No claim that greedy always finds the optimum; exact small-state DP used, no source code copied.

## Build and tests
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/merge-test src/com/gg007/covercress/Board.java BoardTest.java then java -cp /tmp/merge-test com.gg007.covercress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret included. adapter/android is a Java2D drawing adapter used with CoverAdapterTest.java, not an Android runtime.

## Privacy and branding
Covercress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, bundle numbers and solved-level marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon and studio https://ilanis-agent.github.io/gg-007-gaming/.

## Preservation and publishing
Complete source/APK, exact cumulative 236-card studio and publishing fragments privately preserved:
https://files.instinct.com/otw94h67asnr-covercress-source-archive
https://github.com/iLanis-agent/covercress holds README only, full Git source pending. All four existing studio includes and prior card bytes unchanged. Pages settings untouched. Both live sites verified separately.

## Rule sources
https://www.cse.iitd.ac.in/~naveen/courses/CSL758/weighted%20set%20cover.pdf
https://web.cs.dal.ca/%7Enzeh/Teaching/4113/book/dual_fitting/set_cover.html
https://en.wikipedia.org/wiki/Set_cover_problem
https://paal.mimuw.edu.pl/docs/w_set_cover.html
https://cs.ucr.edu/~neal/publication/Young16SetCover.pdf
https://theory.stanford.edu/~trevisan/cs261/lecture08.pdf
