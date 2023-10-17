# Wikipedia Article Quality For US Cities

## Project Goal

The goal for this project is to perform an analysis on ORES data from different Wikipedia articles, particularly on articles that pertain to US cities. The data is being pulled from different places, such as the US Census Bureau, as well as different API calls to Wikipedia (to retrieve the metadata for different pages). Using all of this information, we calculate the the number of high quality articles that are produced when it pertains to different areas of the country. This could highlight glaring disparities and biases when it comes to article quality for different places.

## Research Implications

I have learned a lot from working on this project. I learned that the quality of certain articles can depend on how popular/well known the subject of the article is. Just from a cursory glance at the data, I found that lesser known places seemed to have better article qualities. My hunch is that if people are writing a Wikipedia article about a very niche subject, then there is a lesser likelihood that the article information may be sabotaged. Bigger cities may have a lot more information about them, and thus there would be a higher chance of misinformation being present on them. I also noticed that Wikipedia article titles tend to put the name of the city and the state, unless it was a very well known city.

My results would suggest that English Wikipedia is not credible as a data source, since most of the articles were rated C on the ORES scale, and only around 
25% of articles have a rating of GA or FA. This means that if you are going on Wikipedia, it is highly likely you would encounter a bad article in terms of its quality.

I think this data could potentially be biased when it comes to hypothesis-driven research since it really is relying on article quality and the population of different US states. Other than that, we are having to infer a lot of other things. For instance, part of the analysis involved aggregating the data for different Census Bureau divisions. Since these are wider swaths of land than just a state, there is less richness when it comes to uncovering an insight or a pattern.

I think to we could potentially correct for the limitations and biases by adding more data. Specifically, we would want city-level data, since the articles themselves are pertaining to different cities. We had to aggregate a lot of that information when at the state level, which made it difficult to find any patterns. I would also recommend getting more data on things like incomes of different areas, demographic makeups, and more social data to see if any biases in the article quality of certain places could be motivated by those factors.

## Licenses

According to MediaWiki REST API, articles from the English Wikipedia may be used under the Creative Commons Attribution Share-Alike license. For more information, you can read about their terms of use [here](https://www.mediawiki.org/wiki/API:REST_API#Terms_and_conditions)

## Special Considerations
My Jupyter notebook version is 6.5.2, and it utilizes Python version 3.9.16. Make sure to check the version that you are running under to make sure that the functions are compatible.
Finally, when calculating the ORES scores, be wary of the time it takes to generate them. Since we are utilizing over 22000 API calls to generate each JSON file, it could take up to 5 hours to run each to their entirety.