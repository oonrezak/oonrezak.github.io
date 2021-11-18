## En Passant: An Analysis of Trends and Patterns in Chess

<div class="gridwrapper">
  <div class="one"><img src="../images/enpassantproject/chess_openings.png?raw=true"/></div>
  <div class="two"><img src="../images/enpassantproject/heatmap1.png?raw=true"/></div>
  <div class="three"><img src="../images/enpassantproject/fidescatter.png?raw=true"/></div>
  <div class="four"><img src="../images/enpassantproject/wordcloudpawn.png?raw=true"/></div>
</div>

<br />
### Keywords
* web scraping
* data analysis, statistics, visualization, storytelling
* curve fitting

### Project Summary
For chess games enthusiasts, it is their desire to become good chess players and to be ranked among the best in this tournament. What better way to improve their skills by learning from the world’s best? This report will provide information on proven winning strategy played in this game by the best chess players around the world. This information should help aspiring players to hone their skills and to show that they have what it takes to become champions in the game of chess.

Chess games information were retrieved from the website, Chessgames.com. It has an online database which contains records of chess games played around the world since 1843 and information about world known chess game players. It is also a community with a discussion forum where members can discuss anything about chess. Web scraping using Python’s library BeautifulSoup was used to gather data from the website.

Records of chess games that have taken place since 1843 up to 2019 were retrieved from the website. Information on when and where the game was played, who won and how fast the game was won are all part of the records. From the records, the increase popularity of the game is evident with the increasing number of tournaments being played year on year around the world. Perhaps not surprisingly, records show that player on the White Side wins more times that the player on the Black Side. More so, it can take as few as 1 move to win the game to as most as 228 moves. Champions-wannabee might want to look at how the 1-move games were won.

Player information was also retrieved which includes their FIDE-rating and the number of game played. FIDE which stands for Fédération Internationale Des Échecs is the governing body for international chess competitions. This information showed that there is a correlation with the number of games played with the higher FIDE-rating. Chess game enthusiasts should become followers of and should learn from players with higher FIDE-rating.

The opening moves taken by the players from about 900,000+ chess games were also analyzed. From 20 possible first moves, the move that is most taken by the white player is the pawn moving to E4. This was the first move in 47% of all the games. Further, 38% of the games with this first move were won. The heat maps of the most common first move by both White player and the success of the corresponding game are shown on the report. These are guides to chess players on how to start a game with a high level of probability of winning the game.

Lastly, the discussion forum was reviewed with the objective of learning what are the topics of interest discussed by the members of the site. This information can help interested individuals in using the right keywords to search the forum for tips and techniques that can help them in their journey to become better chess players.

### Links
* [Notebook and Write-Up](/html_previews/enpassantproject/enpassantproject.html)
* [Project repository on github](https://github.com/oonrezak/enpassant_project)
* [Back to Main Page](https://oonrezak.github.io/)