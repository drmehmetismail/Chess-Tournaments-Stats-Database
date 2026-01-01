# Chess Tournaments Analyses with Stockfish

Visit https://mehmetmars7.github.io/ChessDBviewer/ for the most up-to-date dataset.

To replicate and calculate game intelligence (GI) score, missed points, and many other metrics, use the scripts at 
https://github.com/drmehmetismail/Game-Intelligence-for-Chess

https://github.com/drmehmetismail/World-Chess-Championships
1 missed point = making a losing blunder in a winning position. 0.5 missed points = making a losing blunder in a drawn position, or drawing blunder in a winning position. 0 missed points = perfect play.

## Sesse
Special thanks go to Steinar (https://sesse.net/), the owner of the well-known chess computer Sesse, who kindly agreed to share with me detailed raw data for all analyzed moves up to and including December 31, 2024. Under the 'Sesse' folder, I have merged this data into a more user-friendly PGN format. An analysis of these games can be found in the same folder.

The Sesse-as-of-31-Dec-2024 folder contains all games and moves analyzed by Sesse. The Sesse_PV folder contains the same games, but the PGNs also include the principal variation (PV) provided by Sesse.

Use your favorite chess GUI to import these games and explore the variations. To access all games with all variations, including PV and refutation lines, visit:
https://huggingface.co/datasets/drmehmetismail/Chess-Super-Tournaments-Analyzed
Note: Each game file may become significantly large in this case.

Data and analyses are provided “as is”. Rarely, a move may register as a “negative” mistake due to e.g. evaluation jumps between mate and non-mate positions by Stockfish, making acpl negative. I leave this uncorrected, as acpl is not a reliable metric even without such issues, and should not be used to as an accuracy measure.
