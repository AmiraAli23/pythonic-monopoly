# Pythonic Monopoly 
## Toronto Rental Analysis

### Rental Analysis

After importing the data and using the groupby function to group by year, we plot the number of dwelling types on bar charts.

<img width="461" alt="Screen Shot 2022-04-04 at 1 52 01 PM" src="https://user-images.githubusercontent.com/99091066/161602439-0006b872-fb0d-4d72-887c-f9425480a982.png">
<img width="396" alt="Screen Shot 2022-04-04 at 1 52 15 PM" src="https://user-images.githubusercontent.com/99091066/161602473-499e3c66-7e86-491c-a1aa-1eb7933896a4.png">
<img width="417" alt="Screen Shot 2022-04-04 at 1 52 36 PM" src="https://user-images.githubusercontent.com/99091066/161602549-0c22c052-540b-4778-b4b0-f4ac98e05f08.png">
<img width="395" alt="Screen Shot 2022-04-04 at 1 52 48 PM" src="https://user-images.githubusercontent.com/99091066/161602582-b3773c5f-08e9-4dec-ae47-d409d33ec595.png">

Over the years, the number of single, detached houses and apartments with more than five storeys have remained the highest percentage of dwellings. Over time, there is a noticeable gap between the two, that widens as the number of apartments with more than five storeys begins to increase. The number of duplexes have also increased over time. 

Generally, all dwelling types have seen a decrease except for apartments with more than 5 storeys. This can possibly be explained through the increase in immigration, as newcomers with typically opt for affordable living arrangements. Another explanation could be the rising costs of living, which have made home ownership (and even renting) unaffordable.

### Shelter Costs - Owned vs Rented

Here, we compare the costs of renting vs owning property. 


<img width="193" alt="Screen Shot 2022-04-04 at 1 58 14 PM" src="https://user-images.githubusercontent.com/99091066/161603517-31dea95d-4c09-4d06-885f-3e77f1fb7529.png">

<img width="173" alt="Screen Shot 2022-04-04 at 1 58 30 PM" src="https://user-images.githubusercontent.com/99091066/161603563-c684be93-acaf-4430-a4e4-a8dfecf2e29e.png">

Both figures have increased since 2001, however the cost to own a shelter has increased signficantly. Since ownership costs are much higher, people might opt to rent instead. This is further demonstrated when examining the graphs above, specifically the influx of individuals who opt to live in an apartment. 


<img width="419" alt="Screen Shot 2022-04-04 at 2 01 17 PM" src="https://user-images.githubusercontent.com/99091066/161604011-2d771947-69f9-4e79-bb9b-b5edc7b51a7a.png">

  > The dip in housing costs in 2006 can be explained by the 2006 housing market crisis, which eventually lead to the 2007/2008 recession.


### Average House Value Per Year 

Over the span of 15 years, the value of houses in Toronto has tripled. Owning a home is an investment, as we have seen steady growth. As the value increases, the prices follow the same pattern. Those who already own a home are benefitting from the increase, while those who wish to purchase property are now hesitant because of the rising prices. 

<img width="542" alt="Screen Shot 2022-04-04 at 2 02 40 PM" src="https://user-images.githubusercontent.com/99091066/161604207-308da4f1-c0b7-46f9-a95c-1f42a6b6d3f7.png">
 > This figure is nearly a perfect slope of 1


### Average House Value by Neighbourhood 

Using Hvplots, we were able to map the average house value per year, per neighbourhood. The figure below is specific to Danforth, and can be adjusted using the drop down menu.


<img width="843" alt="Screen Shot 2022-04-04 at 2 08 43 PM" src="https://user-images.githubusercontent.com/99091066/161605098-149f8d1c-54a8-49dc-bad2-0e8e918176b2.png">


### Number of Dwelling Types Per Year

Here we are analyzing the number of dwelling types per year, per neighbourhood. 
Below are the ccharts for Scarborough - Village. 

<img width="913" alt="Screen Shot 2022-04-04 at 2 13 17 PM" src="https://user-images.githubusercontent.com/99091066/161605803-99bc2a51-900b-4db6-bcf4-b759d6ccfe37.png">

Apartment complexes over 5 storeys are the most popular in the Scarborough region. 



<img width="834" alt="Screen Shot 2022-04-04 at 2 16 04 PM" src="https://user-images.githubusercontent.com/99091066/161606258-4065d26b-f7ae-442b-8fae-ff20081fbaee.png">

Single detached homes are the most popular type of dwelling in the Lawrence Park North area. 


### The Top 10 Most Expensive Neighbourhoods 

I grouped the data by neighbourhood and found the mean of the average house values per neighbourhood and displayed it in ascending order. The top 10 were selected and graphed on a bar plot. 


<img width="680" alt="Screen Shot 2022-04-04 at 2 19 03 PM" src="https://user-images.githubusercontent.com/99091066/161606725-f821563c-949a-412f-acba-089ebf8c8a6a.png">

Bridle Path has the highest value amongst the other neighbourhoods. When analyzing the dwelling types per neighbourhood, it is clear that Bridle path mostly has single detached homes in the area. Factoring in the massive increase in prices/values of houses over time, it makes sense for Bridle Path to be the most expensive area to live in.

<img width="674" alt="Screen Shot 2022-04-04 at 2 19 29 PM" src="https://user-images.githubusercontent.com/99091066/161606808-4f241255-f919-43a2-b4cd-aef589a2a592.png">



### Neighbourhood Map

After importing the latitude and longitude coordinates per neighbourhood, I combined the `to_data` data frame with `nl` (neighbourgood locations) to form the `combined` dataframe.


Using the Mapbox API, I was able to visualize the average house value per neighbourhood on a map of Toronto. Warmer colours (red, orange, yellow) correspond to a higher property value, whereas cooler colours (blues) represent lower values. The colour tone (dark/light) represents intensity: darker warms signify the highest value, whereas darker cools represent the lowest. Bigger plot points also represent a higher average house value.


<img width="829" alt="Screen Shot 2022-04-04 at 2 26 48 PM" src="https://user-images.githubusercontent.com/99091066/161607949-e646f5d0-8357-452e-b2a2-94001aa8529e.png">

<img width="824" alt="Screen Shot 2022-04-04 at 2 27 31 PM" src="https://user-images.githubusercontent.com/99091066/161608048-d95c66cf-0d65-4f27-9e24-0a232c0d982e.png">

> The darkest and greatest point on the map is Bridle Path, which makes sense when we view the analysis above. 










