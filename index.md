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


<h4>2020-09-29</h4>

I trust that by now you would agree that:

• In the absence of COVID-19 signs and symptoms, Cov-2 positive laboratory tests (e.g., PCR) have limited practical value.<br/>
• New cases, assuming the diagnostic criteria also include COVID-19 signs and symptoms, is an important indicator for resource allocation in the healthcare system but is not a good measurement of pandemic progression as it is confounded by New tests.<br/>
• Total (confirmed, or cumulated) cases is the least relevant indicator for evaluating the current COVID-19 situation. Active cases per million is better as it also factors in recovered cases and deaths and it is normalized to the country population.

For these reasons, the most relevant indicators for pandemic worsening or progression are <b>Positive rate</b> and, to some extent, <b>Active cases per million</b>. We can use these two to create a consolidated indicator, or index: <b>ACPO-14</b>.


<h4>2020-10-01</h4>

<b>ACPO-14</b> stands for "Active & Positive 14 days". It is computed as the product of the average <b>Positive rate</b> and the slope of <b>Active cases per million</b> over the last 14 days (where both data are available; slope computation allows for 1-2 days’ worth of data to be missing at the ends of the 14-day sliding window but this is seldom the case, if at all) or zero, whichever is greater (see update 2020-10-21 further below for revised definition).

The idea behind <b>ACPO-14</b> is simple. Intuitively, the pandemic risk at a particular location increases with the positive rate and the density of active cases. If the positive rate drops to zero (i.e., there is no transmission) then it doesn’t really matter how many active cases there are as no more people will become infected. When the pandemic began, active cases were non-zero and the positive rate was high but the pandemic risk was still minimal as there were not many people who could transmit the infection. Last but not least, on any particular date <b>Positive rate</b> is a property of that point in time while <b>Active cases per million</b> is a reflection of the last six weeks of the pandemic, so together they describe a trend. If this was about people in a room being flooded with water, imagine that the former is the volume of water already in the room and the latter is the speed at which water is flowing into the room: the greater any of them, the higher the risk of drowning soon to the people who are in the room.


<h4>2020-10-14</h4>

It turns out that the ECDC provides some information on COVID-19-related hospital and ICU admissions (EU only). I have considered adding the latter indicator to COV2CON; however, this is problematic as reporting is done in a slightly different manner across EU countries. For example, while 18 EU countries report daily ICU occupancy, the other 8 countries report new weekly ICU cases per 100K people. 

<h4>2020-10-21</h4>

I have revised the definition of ACPO-14 as follows (and updated the executable accordingly): 
>ACPO-14 is the <i>square root</i> of the product of the average <b>Positive rate</b> and the slope of <b>Active cases per million</b> over the last 14 days (where both data are available; slope computation allows for 1-2 days’ worth of data to be missing at the ends of the 14-day sliding window) or zero, whichever is greater.

Here are the current Top-7 countries based on the revised definition:

![Figure 24](/img/img030.png)

The clear "winners" today are Czech Republic, Belgium, and Netherlands.

However, there are countries where the reported data is, let's say, "surprising". It is possible, but unlikely for a country to have a very high positive rate and an extremely low active cases per million. For example, consider Mexico on 2020-10-21: positive rate was at 30% (it was at 40% six weeks before and slowly decreased since then) while active cases per million appears "stuck" at around 350 since July 2020. This apparent discrepancy is difficult to interpret, to say the least. Other countries have either stopped providing positive rate data altogether or have never provided it at all. Compare the sixth image down from 2020-09-17 with the one below and notice that the plot (i.e., the data) for Argentina is gone and the one for Colombia has never been there in the first place; these are not exceptions.

![Figure 25](/img/img028.png)

This is the reason why many countries don't show at the top of the ACPO-14 list, and it also makes country comparison difficult.
