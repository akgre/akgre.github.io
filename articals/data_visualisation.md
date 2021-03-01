# Data Visualization

It's no secret that data can be very powerful — when you can actually understand what it's telling you, that is.

It's not easy to get clear takeaways by looking at a slew of numbers and stats. You need to have the data presented in a logical, easy-to-understand way so you can apply your learnings in an effective way. Using charts, graphs, and design elements, data visualization can help you explain trends and stats much more easily. But, not all data visualization is created equal.

## Real-Life Example

I have created a hypothetical example of a chart that was used in a report.

We are testing three units of the same product that has Wi-Fi and each has 2 outputs. We want to know the transmit power vs channel number of each of the outputs, if they are within set limits and the differences between the output and the individual units.

![wifi_tx_a](C:\Users\Zircon\Desktop\python_projects\akgreenyer.github.io\articals\img\wifi_tx_a.PNG)

At a quick glance we can get an idea that some outputs have higher power than others and it takes a bit more examination to try and understand the differences between outputs or units but it's not very clear; I also can not see if the results pass or fail.



By modifying how the chart plots to include product ID and adding the limits we can instantly pick out more value from the same data.

![wifi_tx_b](C:\Users\Zircon\Desktop\python_projects\akgreenyer.github.io\articals\img\wifi_tx_b.PNG)

Now we are able to see that unit ID_003 fails on both outputs and that output B is higher than output A in nearly all cases. Reporting this to the designer will help them to investigate the causes and improve the design.

## Identify Trends and Outliers

In the simple example above a small change makes a big difference and this becomes more important when gathering a multitude of data points. 

If you were to sift through raw data manually, it could take ages to notice patterns, trends or outlying data. But by using data visualization tools like charts, you can sort through a lot of data quickly.

## The Discovery Process
When discovering your data you don't want your tools slowing you down. This is where I prefer to use data visualisation software like [Tableau](https://www.tableau.com/) over excel.

Most reporting tools require your analyst to know exactly what they’re trying to build before they begin, making initial data exploration a slow process of trial and error.

Tableau’s drag and drop interface allows for anyone to quickly try new ideas, drill into interesting areas and make updates. The ability to rapidly explore and build out visualizations allows for dashboards to provide the most useful and relevant information.

## Reporting 
Once the data of interest has been set they can introduced to the report document.

Tests produce a lot of data that often must be presented to a team so that knowledgeable data driven decisions can be made and fed into the product development lifecycle. To drive consensus among your group, the best way to present data is through reports. Reports can highlight anomalies and help you dig into the details of why a change didn’t perform as expected. Reports can also verify that a change did impact a product positively, such as a performance improvement over the last iteration of a product.
