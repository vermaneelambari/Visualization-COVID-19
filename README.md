# Visualising COVID-19 

##### Within months, COVID-19 went from an epidemic to a pandemic. From the first identified case in December 2019, how did the virus spread so fast and widely? In this R project, I am visualizing data from the early months of the coronavirus outbreak to see how this virus grew to be a global pandemic.

![image](https://user-images.githubusercontent.com/34072722/82515073-2dc34800-9acc-11ea-9d74-af76b634cc3f.png)
#### Manipulating data frames using dplyr and making plots using ggplot2 

## Deliverables: 
#### - From Epidemic to Pandemic 
> I visualized COVID-19 data from the first several weeks of the outbreak to see at what point this virus became a global pandemic. Loading the `readr`, `ggplot2`, and `dplyr` packages. 

#### - Finding out the confirmed cases throughout the world
> Found the cumulative confirmed cases of COVID-19 worldwide by date. Just reading numbers in a table makes it hard to get a sense of the scale and growth of the outbreak. Plotting to visualize the confirmed cases worldwide using `ggplot2`, `geom_line()`.

#### - Comparing China to the rest of the world
> Early on in the outbreak, the COVID-19 cases were primarily centered in China. Let's plot confirmed COVID-19 cases in China and the rest of the world separately to see if it gives us any insight using `tibble`'s `glimpse()` and `ggplot2`'s `geom_line()` functions. 

#### - Plotting the hardest hit countries by Mid-March 2020
> `
confirmed_cases_top7_outside_china <- read_csv("datasets/confirmed_cases_top7_outside_china.csv")
ggplot(confirmed_cases_top7_outside_china, aes(date, cum_cases, color = country, group = country)) + 
geom_line()+ylab("Cumulative confirmed cases") `

![Image](https://user-images.githubusercontent.com/34072722/82515033-12583d00-9acc-11ea-91df-5783458f6050.png)
