<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>NFL Home-Field Advantage</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <header>
        <h1>NFL Home-Field Advantage</h1>

        <p class="subtitle">
            How does home-field advantage vary across NFL seasons
            throughout the last 10 years?
        </p>

        <p class="date">2016–2025</p>
    </header>


    <main>

        <section>
            <h2>Problem Definition</h2>

            <p>
                Home field advantage has been talked about for decades with some people saying it is actually more useful than others. It has been talked about if you actually play better with home fans than being on the road with fans booing and talking bad to you. By looking at NFL game results from the last 10 years and calculating the home team's win percentage for each season, we can see weather it has chnaged over time or not. My research question I will be answering is "How Does Home-Field Advantage Vary Across NFL Seasons Throughout the Last 10 Years?" This question is relevant because it is an important part of understanding NFL games and team performance. NFL teams, players, coaches, fans, and analysts could all be interested in whether playing at homr still provides a significant advantage.
            </p>

            <p>
                This project examines how home-field advantage has changed
                across NFL seasons from 2016 through 2025.
            </p>

            <p>
                The main research question is:
            </p>

            <blockquote>
                How does home-field advantage vary across NFL seasons
                throughout the last 10 years?
            </blockquote>
        </section>


        <section>
            <h2>Data Description</h2>

            <p>
                The data for this project comes from nflverse's NFL
                schedule data. The dataset contains information about
                NFL games across multiple seasons.
            </p>

            <h3>Main Variables</h3>

            <ul>
                <li>Season</li>
                <li>Home Team</li>
                <li>Away Team</li>
                <li>Home Score</li>
                <li>Away Score</li>
                <li>Game Result</li>
                <li>Location</li>
                <li>Season Type</li>
            </ul>

            <p>
                Each row represents an individual NFL game.
            </p>
        </section>


        <section>
            <h2>Data Cleaning & Preparation</h2>

            <p>
                The dataset was cleaned and organized using Python and
                pandas. The analysis was restricted to the 2016–2025
                NFL seasons.
            </p>

            <p>
                Games were grouped by season and the percentage of games
                won by the home team was calculated for each season.
            </p>

            <pre><code>
home_win_percentage = (
    df.groupby("season")["home_team_win"]
    .mean() * 100
)
            </code></pre>
        </section>


        <section>
            <h2>Data Analysis & Visualization</h2>

            <h3>Home Team Win Percentage by Season</h3>

            <img
                src="images/home_win_percentage.png"
                alt="NFL home team win percentage by season"
                class="chart"
            >

            <p>
                The line chart shows how the percentage of NFL games won
                by the home team changed from 2016 through 2025.
            </p>
        </section>


        <section>
            <h2>Findings</h2>

            <p>
                The results show that home teams won more than half of
                NFL games in most seasons during the period studied.
            </p>

            <p>
                However, the size of the home-field advantage varied
                from season to season. This suggests that home-field
                advantage is not a constant value and may change over time.
            </p>
        </section>


        <section>
            <h2>Limitations</h2>

            <ul>
                <li>The analysis only covers ten NFL seasons.</li>
                <li>Home-field advantage can be affected by many factors.</li>
                <li>The analysis does not account for individual team strength.</li>
                <li>COVID-19 affected attendance during some NFL games.</li>
            </ul>
        </section>


        <section>
            <h2>Conclusion</h2>

            <p>
                Home-field advantage has remained an important part of
                NFL games, but its effectiveness has varied across seasons.
                Examining home-team win percentage provides a simple way
                to measure how this advantage has changed over time.
            </p>
        </section>


        <section>
            <h2>References</h2>

            <ul>
                <li>
                    <a href="https://github.com/nflverse/nflverse-data">
                        nflverse Data
                    </a>
                </li>

                <li>
                    <a href="https://github.com/JoshTobin06/Project-1">
                        GitHub Code Repository
                    </a>
                </li>
            </ul>
        </section>

    </main>


    <footer>
        <p>NFL Home-Field Advantage | Data Science Project</p>
    </footer>

</body>
</html>
