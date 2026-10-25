# GameCade A+

GameCade is an Electron-based educational mini-game arcade with a custom game-console + A+ icon.

## Included games
1. Snake Battle — AI opponents, three difficulty modes, mouse steering, and eight-direction movement
2. 2048
3. Brick Breaker
4. Grammar Rush
5. Tetris
6. Sudoku
7. Flappy Flyer
8. Math Sprint
9. Science Showdown
10. History Quest
11. Geo Genius
12. Code Breaker
13. Word Wizard
14. Typing Blitz
15. Memory Matrix
16. Reaction Rush
17. Geometry Dash — jump over obstacles and finish the course
18. Maze Runner — navigate a maze to the exit
19. Space Shooter — dodge enemies and fire shots
20. Racing Rush — avoid traffic and survive
21. Platform Quest — jump and collect stars
22. Puzzle Slide — arrange numbered tiles
23. Hangman — guess hidden words
24. Color Switch — time clicks into a target zone
25. Tower Defense — place towers to stop enemies

Games include a shared 10-level selector. Settings include audio controls, local FPS, and connection estimates.

## Build the Windows installer using GitHub Actions
1. Extract this ZIP.
2. Upload all files and folders to your existing GameCade GitHub repository, replacing the previous project files. Keep `.github/workflows/build.yml`.
3. Commit and push to the `main` branch.
4. Open **Actions** and wait for the Windows build to finish successfully.
5. Open the completed run and download the `GameCade-Windows` artifact. Extract that artifact to find the Windows installer.

You do not need to run `npm start` locally to build the installer.

## Run locally (optional)
Install Node.js, then run `npm install` and `npm start`.

## Notes
- Snake opponents are computer-controlled, not online multiplayer.
- FPS is measured locally. Connection/ping values are estimates, not a full bandwidth test.
- The JavaScript syntax check passed during packaging. The full packaged Windows app has not been runtime-tested here.


## Language learning and sports games

This edition adds five distinct playable experiences: Bahasa Melayu Master (Malay grammar and usage questions), Chinese Character & Pinyin (characters, pinyin, tones, measure words and sentence order), Pronunciation Coach (uses the operating system/browser speech-synthesis voices when available), Soccer Shootout (ten penalty attempts), and 10-Ball Pool (click-to-aim table with simple offline ball physics). Speech voice availability depends on the Windows installation; pronunciation audio is not bundled as prerecorded native-speaker audio.


### Latest quiz/audio improvements
- Code Breaker now has a larger binary/computer-science bank and avoids repeating a question within a 10-question round when the selected stage has enough questions.
- Multiple-choice answers are shuffled on every question while the correct answer remains correctly tracked.
- Chinese and Malay subject banks are selected for questions when translations are available; untranslated subjects fall back to English rather than pretending every item is translated.
- Music and effects default to 100% and use a stronger synthesized gain. Actual loudness still depends on the system volume and speaker hardware.
- Quiz cards and answer buttons have higher-contrast neon styling and clearer hover feedback.
