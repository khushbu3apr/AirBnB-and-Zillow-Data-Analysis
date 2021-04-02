This data analysis is done to consult for a real estate company that has a niche in purchasing properties to rent out short-term as part of their business model specifically within New York City. The real estate company has already concluded that two bedroom properties are the most profitable; however, they do not know which zip codes are the best to invest in. My goal is to build out a data product and provide our conclusions to help real estate company understand which zip codes would generate the most profit on short term rentals within New York City.

I looked at two publicly available datasets, both are in CSV format:
1) Cost Data (Zillow Data) - It provides an estimate of value for two-bedroom properties.
2) Revenue Data (AirBnB Data) - This data provides the attributes of each room/apartment present for renting. AirBnB acts as the medium through which the investor plans to lease out their investment property. 

Assumptions: 
1) The investor will pay for the property in cash (i.e. no mortgage/interest rate will need to be accounted for).
2) The time value of money discount rate is 0% (i.e. $1 today is worth the same 100 years from now).
3) All properties and all square feet within each locale can be assumed to be homogeneous (i.e. a 1000 square foot property in a locale such as Bronx or Manhattan generates twice the revenue and costs twice as much as any other 500 square foot property within that same locale.)
4) Occupancy rate can be assumed at 75% or we can come up with owr own model to calculate occupancy. 

Packages Used:
1) Pandas
2) Numpy
3) Geocoder
4) Geopy
5) Matplotlib
6) Seaborn

Key findings of overall analysis:
Now I have the results from both the scenarios i.e. self calculated occupancy rates and given occupancy rates. If both the results are compared, it shows some disparities in the analysis. When considered self calculated occupancy rates, zipcode 11234 from Brooklyn is shown to be the zipcode with longest breakeven period which is because of the fact that it has low return on cost which in turn comes from very low occupancy rate for this zipcode. This differ from the fact that Brooklyn is one of the most rented boroughs.

I have calculated the occupancy rate depending upon availability of the property for renting. But in real there could be so many exogenous factors affecting occupancy rate. This leads to the disparity. So for the purpose of this analysis and visualizations, I'll use the given common occupancy rate of 75%.


