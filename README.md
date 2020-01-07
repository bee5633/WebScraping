# WebScraping

<b> Introduction </b> \

My interest in port wine began a few years ago when I visited a Long Island winery and had my first taste of very sweet red wine. Back then, I didn't know much about wines and thought all red wines are bitter, so I was pleasantly surprised to discover this sweet taste. I decided to buy that wine and saved it as a treat for my upcoming birthday. This was my introduction to port wine and it has since become one of my favorite wines. For the web scraping project, I used WineEnthusiast Magazine website to compare different port wines. \

<b> Data </b> \

I used Python framework scrapy to scrape the Wine Enthusiast Magazine website that produced two different csv files: an 8.5 MB file with the entire wine dataset and a 1 MB file limited to the port wine dataset. They both included the following information: wine name, wine price, wine category, wine variety, wine origin country, wine origin region, points given by W.E. Magazine and description given to each wine by W.E. Magazine. The image below shows the original website and what kind of information is provided.\

<b> Analysis from entire wine dataset </b> \

First, I wanted to see what defines port wine and how it is different from other types of wines. In order to do that, I used the entire wine dataset. There are three features of wine that I used to compare different types of wines: average wine scores given by Wine Enthusiast Magazine, median price, and median alcohol content (%) in wine. The graphs below show the results. \

From these graphs, it is evident that port wines tend to have higher prices, higher alcohol content and higher scores from W.E. Magazine. This original EDA from the scraped data for all wines shows that port wine seems to be very distinct and highly valued in the wine industry. At this point, I decided to take a more in-depth look at port wines. \

<b> Analysis from Port Wine Dataset </b> \

After the decision to focus on the port wine, I scraped the website again to obtain only the port wines information. From that, I eliminated the wine regions where fewer than 50 port wines are produced to focus my analysis only on the regions that produce a large number of port wines. As a result, there were 2216 port wines in total, out of which 1322 are from Portugal, 648 from the U.S. and the remaining 246 from Spain. By regions, Port and Douro from Portugal, California in the U.S. and Andalucia in Spain produce the most port wines.\

While I was researching the different port wine production regions, the huge differences in production number made me curious to find any other differences between two Portugal regions: Port and Douro. \

I found that the price of port wines produced in two different regions were very comparable, and the points awarded by W.E. Magazines for port wines in two different regions were quite alike as shown in the graphs below. Geographically, these two regions are very close, so the question is: what accounts for the significant differences between them? \

Another interesting thing I noticed while looking into the wines production distribution in different regions was that in Portugal and U.S. there are sub categories of 'port wine' inside the 'port/sherry' category of wine, in contrast to Spain, where 'port wine' does not appear under the 'port/sherry' category of wine, as shown below. \

As a result of my research on this, I found that under European Union Protected Designation of Origin guidelines, only products of Portugal may be labelled as "port" or "Porto". In the United States, wines labelled "port" may come from anywhere in the world, while the names "Oporto". "Porto" and "Vinho do Porto" have been recognized as foreign, non-generic names for port wines originating in Portugal. \

From above, it seems like port wines from Portugal, the original bithplace of that variety, remain very well-received. They are distinguished by their higher alcohol content and higher prices when compared to port wines from the U.S. and Spain, as shown in the graphs below. \

Given that port wines are distinguished by higher prices and higher alcohol content than other wines, should we conclude that the higher alcohol content is what makes it expensive? According to the scatter plot below, that is not the case. Port wines usually contain about 20% alcohol content, and higher prices were all concentrated at 20%. \

How about the ages of the port wine? Would that be a factor in the price? The scraped information didn’t include the produced year information; however I created another column using the year that was included in the name of some of the wines. Age does seem to elevate price when you look at the port wines from Portugal, though not necessarily for the ones from Spain and the United States. Below is the scatter plot of port wines produced in different years color coded by different countries. Portugal, which is represented by blue shows higher prices for the older wines. On the other hand, red and green colors that represent Spain and the United States do not. \

Lastly, I created a word cloud using descriptions from both the entire wine dataset and the port wine scraped data. I felt the need to compare the word cloud of port wines to those of all wines for a proper comparison. In contrast to general wine descriptions, port wine descriptions had more words like ‘sweet,’ ‘port,’ ‘acidity,’ ‘sweetness’ and ‘chocolate’ which illustrate the sweet characteristics of port wine well. \

<b> Conclusion </b> \

From data analysis, it was clear that port wines are very distinct from other types of wines. Port wines usually refer the port/sherry wines from Portugal in the Douro and Porto regions that have alcohol content of about 20% and higher prices than their Spanish and American counterparts. However, the port wines from Douro seem to have a similar rating given by W.E.Magazines paired with a lower price compared to the ones from Porto. So if you want to taste sweet port wine but don't want to shell out too much for a bottle, you may consider the ones from Douro. I hope you enjoy your port wine!
