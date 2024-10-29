---
layout: post

title: "Unveiling the Secrets of Orange County's Housing Market: A Data-Driven Analysis"
author: Samantha Richardson
description: "Discover what drives housing prices in one of California’s most sought-after regions. In this post, we’ll dive into an analysis of how factors like city, square footage, and home features impact affordability in Orange County—providing insights that could help you make informed decisions about where to live after college."
image: /assets/images/orange_county1.jpg
---
<img src="https://samrich277.github.io/my-blog/assets/images/house.png" alt="House" style="width:350px; float: right; margin-left: 15px;"/>

Growing up in the sunny neighborhoods of Orange County, California, I always imagined moving back someday—if I could find something in this wild housing market! With homes that range from cozy to luxurious (and price tags that match), navigating the OC real estate scene can feel like a game. In this project, I dive into the data to decode the trends behind these sky-high prices, exploring everything from square footage to location. Whether you're a hopeful buyer like me or an investor with an eye on the prize, let’s uncover what makes Orange County’s market tick.

---

## Motivating Question

The primary question guiding this project is: 

**What are the key factors that influence housing prices in Orange County?**

## Ethical Considerations and Scraping Best Practices

Before diving into data collection, it's essential to consider ethical guidelines and best practices for web scraping:

- **Respect Website Policies**: Always check the website’s `robots.txt` file to ensure that scraping is allowed.
- **Minimize Server Load**: Use a headless browser and implement delays between requests to avoid overloading the server.
- **Data Privacy**: Ensure that any personal data collected is anonymized and handled in compliance with privacy laws.

## How to Get Started: Step-by-Step Guide

If you want to embark on a similar data project, follow these steps:

1. **###Choose a Target Website**: 
    - Ensure it provides publicly accessible data and that its `robots.txt` file doesn’t prohibit scraping.
    - I found my Orange County housing data from [Houzeo](https://www.houzeo.com/homes-for-sale/california/orange-county)
2. **Set Up Your Environment**:
    - Install Selenium and a web driver like [ChromeDriver](https://developer.chrome.com/docs/chromedriver/downloads/version-selection).
    - Use a headless browser to reduce server load.
    - Import the necessary libraries. 

![imports](https://samrich277.github.io/my-blog/assets/images/imports.png)

3. **Write the Scraping Code**:
    - Identify the relevant HTML elements (e.g., price, address, city, beds, bath, square feet) using browser developer tools.

![main](https://samrich277.github.io/my-blog/assets/images/main_code.png)
    
    - Implement pagination to navigate through all pages of listings.

![paginate](https://samrich277.github.io/my-blog/assets/images/paginate_code.png)

4. **Clean the Data**:
    - Remove any unwanted symbols (e.g., dollar signs) and convert text values (e.g., "5 bds") to integers.
    - Handle missing or invalid data appropriately.
5. **Store the Data**:
    - Save your cleaned dataset as a CSV file for further analysis.

## Summary of the Dataset

The final dataset includes the following variables for each property:

- **Price**: The listing price of the house, converted to numeric format.
- **Address**: The full address, with the city extracted separately for analysis.
- **City**: The city within Orange County where the property is located.
- **Beds**: The number of bedrooms.
- **Baths**: The number of bathrooms.
- **Square Feet**: The total square footage of the property.

## Summary Statistics and Visualizations

- **Mean Price**: $1,250,000 (example value)
- **Median Square Footage**: 2,500 sqft
- **Distribution of Bedrooms and Bathrooms**

!Distribution of Bedrooms
!Distribution of Bathrooms

## Conclusions and Next Steps

The data reveals that ___ are significant factors influencing house prices in Orange County. The scatter plot highlights a clear trend: ___.

## Further Information and Resources

- For a detailed guide on web scraping best practices, check out Web Scraping Best Practices.
- To explore the dataset further and access the code, visit my GitHub repository.
- Learn more about real estate data analysis here.

---

By following these steps, you can start your own project to analyze housing prices in Orange County. Happy analyzing!


