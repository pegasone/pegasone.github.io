# PROJECT COV2CON

<a href="https://github.com/pegasone/cov2con">Cov-2 Condition</a> — A visualization and exploration instrument for COVID-19 pandemic data. The Gallery that follows is a suite of screenshots taken in this Windows 10 Desktop app.

<h3>GALLERY</h3>

<h4>2020-09-17</h4>

Let's start with this graph for Qatar, which tops the list of countries ordered by <b>Total cases per million</b> population.

![Figure 1](/img/img002.png)

It shows that in Qatar this indicator rose fast in May-June 2020 and then it slowed down to a plateau. So, Qatar should be in pretty bad shape by now (Sep 2020) one would think, right? Not really. Let's have a look at <b>Active cases per million</b>.

![Figure 2](/img/img004.png)

Notice how this indicator dropped dramatically after peaking out at the beginning of June. Let me rewrite this: after reaching around 12000 active cases/million on 2020-05-27, this indicator dropped tenfold by mid-July and remained stable since then. How is this possible? Let's have a look at the <b>Positive rate</b>.

![Figure 3](/img/img003.png)

It shows that Qatar successfully controlled the transmission of the disease beginning in July. <b>Active cases per million</b> dropped almost in sync with the <b>Positive rate</b>.

Let's see what the situation was like at that time in a few other countries: Unites States, France, Spain, Netherlands, Sweden, and Israel. I chose these countries because they too are near the top on the <b>Active cases per million</b> list, as can be seen on the heat map.

![Figure 4](/img/img012.png)

<b>Active cases per million</b> were almost flat in June-July in Israel, Spain, France, and Netherlands while they were increasing fast in Qatar, Sweden, and the United States.

Qatar notwithstanding, Sweden and the United States appear to have the highest <b>Positive rate</b> numbers in June-July (some the data for Sweden is unavailable).

Notice how numbers blow up again in early September in Spain, France, and Israel. United States and Netherlands seem to have more control over the situation while Sweden and Qatar are in the best positions.

![Figure 5](/img/img011.png)

![Figure 6](/img/img013.png)

These plots also suggest that, an almost flat <b>Active cases per million</b> curve is consistent with a <b>Positive rate</b> of 1%-2%. At a rate of 4% and above it seems almost impossible to stop the daily increase in active cases. 

Central and South America during this time tell us a very different story... More on this later.

![Figure 7](/img/img006.png)

Let's see how The Five Eyes did. One country leads the pack, and at a first glance it would seem that <b>Positive rate</b> can explain the big differences.

![Figure 8](/img/img014.png)

![Figure 9](/img/img015.png)

However, if we overlay <b>Positive rate</b> and <i><b>New cases per million</b></i> (not presented in COV2CON), we notice the latter increased faster than the former in June-July. 

![Figure 10](/img/img001.png)

This is likely due to an increasingly high number of tests conducted in that country in June-July, peaking end of July, as communicated in the [media](https://www.statista.com/statistics/1111601/covid-19-tests-carried-out-daily-in-the-us/).

![Figure 11](/img/img016.png)


<h4>2020-09-23</h4>

What is this entire ruckus about a new wave of COVID-19? Let's have a look at the data in Europe and North America.

I'm cherry-picking 7 countries in Western Europe: Netherlands, France, Germany, Spain, Italy, Austria, and Switzerland.

![Figure 11](/img/img017.png)
![Figure 12](/img/img018.png)

It's interesting that Germany can act as a "negative control" and Spain maybe as a "positive control" (if you are a Biologist, you know what I mean), in this case. Clearly there is an increase in positive rate in most of these countries, which matches spikes in active cases per million in Netherlands, France and Spain.

How about Central Europe? Here comes another round of pick-and-choose: Poland, Czech Republic, Slovakia, Hungary, Croatia, Serbia, and Slovenia.

![Figure 13](/img/img019.png)
![Figure 14](/img/img020.png)

A trend similar to the one in Western Europe is observed in Central Europe, with spikes in active cases per million in the Czech Republic and Hungary, and somewhat less in Poland and Slovakia. The plot sections for Serbia are inconsistent though.

Now in Eastern Europe: Belarus, Ukraine, Romania, Bulgaria, Moldova, and Macedonia (with the caveat that positive rate data is not available for Moldova and Macedonia).

![Figure 15](/img/img021.png)
![Figure 16](/img/img022.png)

While Belarus looks in surprisingly good shape, the other 4 countries not so much, particularly Ukraine and Moldova. Romania shows an unexpected recent drop in active cases per million that is difficult to interpret.

Wrapping up this region is Northern Europe: Norway, Denmark, Sweden, Finland, Estonia, Latvia, and Lithuania.

![Figure 17](/img/img023.png)
![Figure 18](/img/img024.png)

Interesting: almost flat and close to zero positive rate curves and yet big spikes in active cases per million in Sweden and Denmark. This could simply mean that these two countries have recently tested a lot more people than before, but it's a trend to watch.

Finally, let's take a look at North America: Canada, United States, and Mexico.

![Figure 19](/img/img025.png)
![Figure 20](/img/img026.png)

I see a big discrepancy here: in the US, the positive rate remains quite elevated, and they likely continued to conduct a lot of tests, which would help explain the spike in active cases per million. However, in Mexico the positive rate is at "historically" low rates and yet active cases per million have dropped almost to zero? Well, this would be possible I guess if they conducted only a few tests per day. Sure...

Okay, so what I see is recent spikes in positive rate and active cases per million in a few but not all European countries. Next week we'll hopefully know more.


<h4>2020-09-24</h4>

Here is a heat map of <b>Active cases per million</b>, updated today. The overall appearance has not changed much from one week ago. The closer to yellow the colour of a country on the map, the higher the likelihood that you would find yourself surrounded by people who have tested positive for COVID-19 (molecular test; clinical manifestation not implied) should you travel to that country in the near future.

![Figure 21](/img/img027.png)


<h4>2020-09-26</h4>

By now you must have realized that, not all countries provide data for each of the three indicators and on each day. You may be wondering, how can one quickly find  countries where the COVID-19 situation has recently gotten worse? Here is one way to do it.

Head over to the active cases per million indicator. It is very likely that all countries will show "no data" on the current date (i.e., default date when launching the app). This is normal because the values of this this indicator are parsed off of JHU data sets, which are based on data available on the previous day. Use the slider to change the date and go back one day; for example, if today's date is 2020-09-26, change the date to 2020-09-25. Now most countries on the list show numerical values instead of "no data", and country names are listed in descending order of these values. Select a few items at the top of the list. Examine the historical data graph and make a note of the countries with recent spikes in active cases per million. In the example below, these would be Spain, Costa Rica, France, Israel, and Belgium. 

![Figure 22](/img/img028.png)

Without changing the  selection, switch over to the positive rate indicator. On the updated graph, make a note of those countries that show recent increases, however small but above 2%, in the positive rate. In this example, these are Spain, France, Israel, and Belgium; alas, there are no positive rate data available for Costa Rica. 

![Figure 23](/img/img029.png)

For consistency, we need both criteria to be met. By cross-referencing the two results we get: Spain, France, Israel, and Belgium. 

By repeating these steps further down the country list we get: United Kingdom, Netherlands, Czech Republic, Ukraine, Portugal...


<h4>2020-09-29</h4>

I trust that by now you would agree that:

• In the absence of COVID-19 signs and symptoms, Cov-2 positive laboratory tests (e.g., PCR) have limited practical value.<br/>
• New cases, assuming the diagnostic criteria also include COVID-19 signs and symptoms, is an important indicator for resource allocation in the healthcare system but is not a good measurement of pandemic progression as it is confounded by New tests.<br/>
• Total (confirmed, or cumulated) cases is the least relevant indicator for evaluating the current COVID-19 situation. Active cases per million is better as it also factors in recovered cases and deaths and it is normalized to the country population.

For these reasons, the most relevant indicators for pandemic worsening or progression are Positive rate and, to some extent, Active cases per million. We can use these two to create a consolidated indicator: ACPO-14.


<h4>2020-10-01</h4>

ACPO-14 stands for "Active & Positive 14 days". It is calculated as the product of the average Positive rate and the slope of the Active cases per million over the last 14 days (where both data are available; the slope allows for 1-2 days worth of data to be missing at the ends of the 14-day sliding window but this is seldom the case, if at all) or zero, whichever is greater. Here is the first screenshot:

![Figure 24](/img/img030.png)

This graph indicates a COVID-19 pandemic worsening in the last 14 days in the following countries: Spain, Israel but also France, Czech Republic, Netherlands, Hungary, and Belgium. Tunisia and Lybia were skipped due to data inconsistencies.

For reference, the corresponding screenshots of Positive rate and Active cases per million are included.

![Figure 25](/img/img031.png)
![Figure 26](/img/img032.png)

This is work in progress and the exact definition of the ACPO-14 indicator may undergo further optimizations. Enjoy the (map) view! ;)

![Figure 27](/img/img033.png)


<h4>2020-10-02</h4>

I have recently had a conversation with someone who thinks the reported numbers for their country are wrong because "they don't make sense". Specifically, they think that active case numbers should have decreased after the first peak; apparently, this assumption is not consistent with the recovered cases and deaths reported for their country. 

As I mentioned before, while the positive rate remains above 2% and many PCR tests are carried out, the active case count does not seem to decrease; further research is required for confirmation.

I have come to realize that what I am trying to do with ACPO-14 is not so different: finding a consolidated, artificial indicator that fits my intuition of the pandemic progression. Now I think that my approach was wrong. However incomplete and inconsistent, reported data comes first and one cannot ignore it. For this reason, I have stopped trying to find an acceptable consolidated indicator. 

ACPO-14 is to stay in COV2CON and I shall update the app only if bugfixes are needed but otherwise I will not develop it any further.