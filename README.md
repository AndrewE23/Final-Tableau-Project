# Final-Project-Tableau

## Project/Goals
While I can summarise my goal as "use Tableau to examine different statistics on Tuberculosis (TB) throughout the world, I would rather elaborate a bit on that by instead framing it as me wanting to explore trends and work toward answering my hypothesis: As initiatives toward fighting TB increase, the prevalence and incidence rates of TB will diminish over time. 

Additional questions and answers follow later.

## Process
### Data Exploration
The short of this is that I experimented with different plot types and even opened the dataset in Excel to gain a better understanding of what I had to work with. We have regions as well as countries, years from 1990 to 2013, as well as various statistics for incidence, prevalence, and mortality rates of TB across these dimensions.

In short, I needed to know what data I had, what data types they were, and whether I would have to make any adjustments; I did not.

### Plot/Graph Creation
To start with, I set up a geographical heat map where I could see TB incidence rates by country, which was soon replaced with a symbol map so I could also render a correlation between symbol size & colour and the actual incidence rates (i.e. bubbles are smaller and lighter for lower rates, while for higher rates they are larger and darker). This data can be adjusted by year to show national shifts.

I followed this with a bar plot, showing the total number of TB deaths each year while also generating a bit of a forecast to work with. 

However, this forecast couldn't give me much insight about possible variances (i.e. it gave very precise numbers), so I made a line plot where I could generate trends and also see how Tableau forecasted the following four years into the future; that let me see that it considered the HIV- forecast much more accurate than the forecast for HIV+ deaths, where there was a lot more room for error. I also decided to make this plot give me average deaths by country as opposed to total deaths, so that my original plot could still serve a valuabel purpose in highlighting global death counts.

After this, I made a scatter plot to show me how different countries (colour-coded by what region they are located in) compare to one another in terms seeing how many TB cases lead to death. Like the first plot, this one can be adjusted by year to show how these comparisons shift across time.

I then made a second scatter plot with the express purpose of comparing case detection rates (filtered to a maximum of a 100% detection rate) to TB incidence, again allowing it to be adjusted by year to see how things change. I also assigned clusters to it so that I could better see how TB rates vary depending on detection rates, defining three clusters so that the data would be easier to recognise a pattern. 

Lastly, I made a simple table showing both the types and use counts of different methods (e.g. for determining incidence/prevalence/mortality rates). However, I found it difficult to work this data into a better visualisation for the dashboard so I excluded it from that; while the insights I gained from it helped me, the table itself is not stakeholder friendly so I decided to lead with what visuals I thought told a more compelling story.

### Dashboard Creation
I then put my five best visualisations together into my dashboard, keeping the more interactive plots on the left side so that viewers' eyes do not have to bounce around when the year slider is adjusted. 


## Results
I chose Option 2, using the TB dataset with which to create my visuals and work through some questions I started to formulate as I worked on it.

Hypothesis: Supported; the available patterns show a correlation between increased detection rate (often through testing), which in turn lowers the incidence and mortality rates. Countries that do not have adequate means of detecting TB cases tend to have a higher prevance of TB. 

1. My main data question was that I wanted to see what the trends were in terms of TB incidence and deaths in different parts of the world (tying into my hypothesis). Is the prevalence of TB, plus the corresponding mortality rate, going down?

Answer: TB has been declining in most of the world, with a few notable exceptions.

2. Which regions of the world have been impacted the hardest?

Answer: Southern Africa in recent years, although SE Asia and Central Africa were hit harder throughout the 1990s. 

3. What can the immediate future (pretending that the current year is 2013 rather than 2023) be expected to look like if current trends continue?

Answer: Overall, TB will continue to decline if current efforts to fight it continue.

I followed along with the prompts in a fairly linear fashion, although I started formulating my questions (prompt 8) well before I finished building my 5 different visualizations (prompt 2) because I wanted to be sure that what I generated would actually help answer my questions as opposed to simply helping me visualize the raw data. The order in which I created my plots is outlined as part of my overall process.

Aside from that, there was little data I needed to join because everything was already connected, and I reviewed the data types I had available to confirm that I did not need to worry about changing anything.


## Challenges 
I initially started with Option 1, which I abandoned halfway through as mild struggles became moderate hurdles, which in turn became major headaches. It was bad enough that my PC hated my efforts to form relationships with as many tables as I did when trying to map out HPI and relative price differences across different regions, but then I got to the JSON file and decided that I wanted a change of pace seeing as I would have had to spend even more time cleaning the data that was provided to me; even if I did so, I could tell that I was going to continue having technical issues even had I spent time doing that.

On the other hand, Option 2 did not give me very many issues. The dataset I chose was fairly straightforward, and what gaps there were in my tables could easily be filled using calculated fields (for example, joint death counts that included estimates for total death count, not just with or without HIV). That said, I wasn't sure how to really utilise the data on what methods were used to test methods for deriving incidence or mortality rates, so I settled for a simple chart to meet one of the criteria listed in the assignment overview.

## Future Goals
Of course, while I did enjoy working with the TB dataset, I also found it sort of barebones in terms of what kinds of data were supplied. For example, there was nothing involving economic data (e.g. GDP, CPI), nor was there anything non-TB related like life expectancy. There was also no real way to distinguish between, say, rates among male and female patients, or even among different age groups. If I were to continue working with the data, I would like to also work with some other metrics so that I could (hopefully) create visuals that tell a fuller story.
