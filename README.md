# Stream Web Scraping

<b>The Project</b> is to a 4 days project on web-scraping, to derive insights from data, presenting it to our imaginary client. It is our first project after a month of first hand experience on Python language, Pandas, Seaborn, Matplotlib, BeautifulSoup, and API Requests. We did plan a 4-days project flow, the flow of the project was well respected while the timeline is adjusted according to challenges. Web-scraping challenges is real, data-cleaning is a challenge. It is now a reminder that data sourcing and data cleaning had taken 85% of our time as a team.

<b>The Project Responsibilities.</b> Initially we explored different ways to source information via get API on Steam Online Game website. On focus, David is responsible for the main framework of the code such as Get API. Mandy manages the project throughout and reminds us with our progress, also on deriving data insights for better business decision, myself Hui-Ee has get together information to create a compelling presentation. I dive deep into our project flow to study the formation of Steam ID, increasing our project flow and accuracy in data source.

<b>My group members are</b> David Chueng [cheungyuk123@gmail.com], Mandy [mandy200525@gmail.com], and Hui Ee [huiee.wong@gmail.com]

<b>The Project Challenge</b> is to acquire a valid Steam ID (gamer ID) for gamer statistical information, as we have to input Steam ID to get the API key. Generating steam ID is a challenging part. The Steam ID itself has 17-digit random ID. By observing a pattern, the first 9-digits of ID are similar while the last 8 digits are random. By decoding the formation, we convert the Steam ID into 64-bit number and convert it back to 17-bit. Ultimately getting Steam ID with 99% account with valid gamer statistical information such as gamers played games, gamers location, total time spent, and money spent.

<br>
<img width="600" src="https://user-images.githubusercontent.com/70442354/202737071-0f5a2b32-a734-4fac-9460-a7a6d166df61.JPG">
<br>

<h3>Project Framework -- Data Collection</h3>
<img width="800" alt="Screenshot 2022-11-18 at 11 06 41 PM" src="https://user-images.githubusercontent.com/70442354/202737569-73a004c7-5857-40e5-9742-c81a596b4b60.png">

<h3>Get Stream Community ID</h3>
<b>Approach 1</b> --- generate random account numbers<br>
<ul>
<li>by observation, valid steam IDs usually have a pattern (e.g. 76561198XXXXXXXXX)</li>
<li>"76561198" + randomly generate 9-digit numbers</li>
  </ul>

<br>
<b>Results</b> --- Extremely low efficiency<br>
(i) < 1% of SteamIDs generated are valid<br>
(ii) Time required to select valid id (~1 valid ID/ second)

<b>Approach 2</b> --- generate the ID from its simple format (i.e. STEAM 1:1:66138017)

<h3>Transforming SteamID to 17-digit number</h3>
<img width="1440" alt="Screenshot 2022-11-18 at 11 28 56 PM" src="https://user-images.githubusercontent.com/70442354/202741106-c7442468-6963-465f-a7c3-52f7a44111ac.png">


<h3>Meaning of the simple SteamID</h3>
<img width="800" alt="Screenshot 2022-11-18 at 11 27 13 PM" src="https://user-images.githubusercontent.com/70442354/202740772-5ee52b74-4e94-44f6-bb37-3c9acd0ddde7.png">


