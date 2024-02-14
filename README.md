# DSC10
 Assignments from DSC10 at UCSD

This first course in data science introduces students to data exploration, statistical inference, and prediction. It introduces the Python programming language as a tool for tabular data manipulation, visualization, and simulation. Through homework assignments and projects, students are given an opportunity to develop their analytical skills while working with real-world datasets from a variety of domains.

 Midterm Project:
 - The project is divided into four main sections, each of which contains several questions.
     - Section 1: Data Visualization
         - In this section, we'll use the tswift DataFrame to create visualizations that will help us answer questions about Taylor Swifts's music, including:
             - How many songs did Taylor Swift release each year?
             - How do different audio features such as "Loudness" and "Energy" relate to one another?
             - Are Taylor Swift's songs generally more positive or more negative?
             - Which Taylor Swift album has the most songs in a minor key?
     - Section 2: Song Recommender
         - In this section, we'll create a Taylor Swift song recommender tool. The tool will allow you to input a song you like, selected from a collection of popular songs on Spotify, and it will recommend to you the songs in Taylor Swift's body of work that are most similar to your input song.
     - Section 3: Lyric Searcher
         - In this section, we'll create a Taylor Swift lyric searcher.
     - Section 4: Keywords
         - In this section, we'll identify keywords that summarize each song in Taylor Swift's album "Lover".

 Final Project:
 - Leverage meteorite data to conduct hypothesis testing and probability analysis, uncovering statistical patterns that contribute to a deeper understanding of celestial events and their potential impact on Earth.
 - This project is divided into six main sections, each of which contains several questions.
     - Section 1: Seen vs. Recorded
         - Let's start by exploring where meteorites were seen falling where they were recorded.
     - Section 2: The View From Space
         - In Section 1, you may have noticed that the map that depicted the location of each meteorite seen falling looked a lot like a world population map. A likely explanation for this is that a meteorite is more likely to be seen if it falls near a populated area. In fact, the map you saw in Section 1 looks very similar to this composite image of the Earth at night – the nighttime lights show areas that are densely populated.
         - We might suppose that the number of meteorites spotted in a continent is proportional to the population of the continent, but this is not quite right. Consider, for instance, Asia, which has the greatest population out of any of the continents, by far. This population, however, is not spread evenly over the surface of the continent – it is concentrated in several areas. We can see this in the nighttime image above – large parts of Asia (such as Siberia, Mongolia, and Western China) are relatively sparsely inhabited.
         - Instead, we might suppose that the number of meteorites seen in a continent is proportional to the total area of the continent that is "sufficiently populated". One way to do this is to count, for each continent, the number of pixels in the above image which are brighter than some threshold. The more bright pixels, the more land area that is populated, and the more surface area where a falling meteorite is likely to be seen.
     - Section 3: Long-Distance Relationship
     - Section 4: Around the World
         - Here's a potentially interesting observation: the median mass of meteorites seen falling in Asia is larger than the median mass of meteorites seen falling in North America.
         - Is there a real difference between the mass of meteorites seen falling in Asia and those seen falling in North America? Or is the observed difference solely due to random chance? Let's investigate this using a hypothesis test once again. Here are our hypotheses:
             - Null Hypothesis: The masses of meteorites seen falling in Asia come from the same distribution as the masses of meteorites seen falling in North America.
             - Alternative Hypothesis: The median mass of meteorites seen falling in Asia is larger than the median mass of meteorites seen falling in North America.
     - Section 5: Confidence is Key
         - Again, saw_fall only contains the meteorites that were seen falling. However, it does not contain information about all meteorites that fell in a given continent, because many meteorites fell but were not seen. In this way, saw_fall contains a sample of the meteorites that fell in each continent.
         - As such, we might be interested in determining an estimate for the true median mass of all meteorites that have fallen in a given continent, given just the information in saw_fall. Sounds like it's time to bootstrap!
     - Section 6: Decade-nt
         - In this question – the final question of the project – we will explore whether there is a trend in the median mass of meteorites over time. As before, we will restrict our analysis to only the meteorites that were seen while falling (i.e. only the meteorites in saw_fall). Furthermore, we will only consider the meteorites that were seen falling since 1900 (including the year 1900).
