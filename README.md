# Information Systems Management Portfolio

Welcome to my portfolio!
I am a Master's student in Information Systems Management (MSI). 
My academic and project background bridges the gap between technical architecture and business strategy.
I specialize in designing robust information systems, driving digital transformation, and leveraging data to support strategic decision-making. 
Below is a collection of projects demonstrating my ability to manage the full lifecycle of digital solutions, from database conception to user-centric innovation.

-----

## Table of Contents

**1.  AFIHM Database Optimization & SQL Implementation
2.  Determinants of Phytopharmaceutical Purchases
3.  Hedonic Price Analysis of Laptops
4.  L'Art Sucré de France (Web & Data Collection)
5.  L'Art 2 la Main (Digital Strategy Consulting)
6.  MagiCouture (Business Innovation)**

-----

## 1\. AFIHM Database Optimization & SQL Implementation
  
**Tools:** SQL (MySQL), Draw.io (MERISE/EER), Relational Algebra

### Project Goal

The AFIHM association suffered from data redundancy and integrity issues due to scattered datasets (Excel files duplicated by year, inconsistent member tracking) . The goal was to redesign their entire data architecture to centralize member management, conference registrations, and complex billing systems .

### Methodology & Techniques

  * **Conceptual Modeling (CDM):** Designed an Entity-Relationship (EER) diagram to map complex relationships, such as distinguishing between "Persons" and "Members" using inheritance/specialization .
  * **Normalization:** Applied **3rd Normal Form (3NF)** to eliminate redundancies. For example, I separated "Events" from "Participation" to allow flexible tracking of workshops and galas without altering the table structure annually .
  * **Constraint Implementation:** Enforced data integrity using **Check Constraints** (e.g., ensuring a payment line refers to *either* a membership *or* an event registration, but not both) and Unique Keys .
  * **SQL Analytics:** Developed complex queries to solve specific business problems, such as calculating total revenue per conference year or listing dietary restrictions for gala logistics .

### Key Competencies

  * **Database Design:** Transitioning from unstable flat files to a normalized relational schema.
  * **Complex SQL:** Writing joins across 4+ tables, using subqueries, and aggregate functions (`SUM`, `COUNT`, `GROUP BY`) .
  * **Data Integrity:** Managing Foreign Keys and Exclusion Constraints to prevent data corruption.

-----

## 2\. Determinants of Phytopharmaceutical Purchases
  
**Tools:** R (tidyverse, lmtest, sandwich), RMarkdown, Excel

### Project Goal

To analyze the economic and environmental factors influencing pesticide purchases by French municipalities in 2022. The study aimed to determine if tax policies or health impact awareness effectively reduced chemical usage .

### Methodology & Techniques

  * **Data Wrangling:** Constructed a massive cross-sectional dataset (5,804 observations) by merging purchase volumes, agricultural surface area (SAU), and weighted tax data based on postal codes .
  * **Econometric Modeling:** Developed multiple regression models, progressing from Level-Level to **Log-Level** to interpret semi-elasticities.
  * **Non-Linear Analysis:** Introduced quadratic terms for taxes to test for "threshold effects" (saturation points where taxes become effective) .
  * **Robust Testing:** Detected heteroscedasticity using **Breusch-Pagan** and **White tests** and corrected the model using **Heteroscedasticity-Consistent (HC) standard errors** to ensure statistical validity .

### Key Competencies

  * **Statistical Inference:** Hypothesis testing (Student t-test, Fisher F-test) to validate model significance .
  * **Policy Analysis:** Concluded that "surtaxes" on specific chemical mentions were effective, whereas general taxes had a counter-intuitive positive correlation due to inelastic demand .
  * **Data Cleaning:** Handling missing values and aggregating disparate data sources.

-----

## 3\. Hedonic Price Analysis of Laptops
  
**Tools:** R, Gretl, OLS Regression

### Project Goal

To build a predictive pricing model for laptops by isolating the marginal monetary value of specific technical features (RAM, Weight, CPU Frequency) using a dataset of 1,265 observations .

### Methodology & Techniques

  * **Feature Engineering:** Created dummy variables for categorical data (e.g., Brand/Company) to measure the "Apple premium" effect .
  * **Model Specification:** Utilized a **Log-Linear regression model** to normalize price distribution and interpret coefficients as percentage changes .
  * **Interaction Effects:** Modeled the interaction between `CPU` and `RAM` to capture how the combination of high-performance components affects price differently than the sum of their parts .
  * **Bias Correction:** Identified heteroscedasticity in the residuals and applied robust standard errors to correct the variance-covariance matrix .

### Key Competencies

  * **Predictive Modeling:** determining that weight has a non-linear relationship with price (value decreases with weight, but stabilizes for very heavy workstations) .
  * **Regression Analysis:** Interpreting coefficients (e.g., 1 additional GHz of CPU adds \~71% to the price) .

-----

## 4\. L'Art Sucré de France (Web & Data Collection)
 
**Tools:** Python (Web Scraping), API (Data.gouv.fr), HTML5/CSS3, Flourish

### Project Goal

To develop a responsive single-page website dedicated to French pastry culture, featuring a data-driven "Tour de France" map that visualizes the location of top bakeries across the country .

### Methodology & Techniques

  * **Data Extraction (ETL):** Built a Python pipeline to scrape content regarding pastry types and integrated the **Sirene API (Data.gouv.fr)** to fetch real-time geolocation data of 25 registered patisseries .
  * **Data Cleaning:** Parsed complex JSON responses from the API, specifically extracting nested coordinates (latitude/longitude) from the "headquarters" nodes to format them for visualization tools .
  * **Visualization:** Injected the cleaned data into **Flourish** to create an interactive map embedded in the site .

### Key Competencies

  * **API Integration:** Handling JSON data structures and RESTful requests.
  * **Web Scraping:** Automating data collection for content generation.
  * **Frontend Development:** Using CSS Grid/Flexbox and 3D animations for interactive data presentation .

-----

## 5\. L'Art 2 la Main (Digital Strategy Consulting)
 
**Tools:** Meta Business Suite, Gantt Charts, SWOT Analysis

### Project Goal

A consulting project for a local pottery artisan ("Florence De Palma") to revitalize her digital presence. The goal was to modernize her brand image to attract a younger demographic and streamline her customer communication .

### Methodology & Techniques

  * **Strategic Diagnosis:** Conducted a **SWOT analysis** to identify the gap between her high-quality craftsmanship and her poor digital visibility compared to local competitors .
  * **Action Plan:** Developed a Gantt chart to structure the deployment of a new website, logo redesign, and social media content calendar .
  * **Automation Strategy:** Set up tools like Meta Business Suite to allow the client to schedule posts in advance, ensuring the strategy was sustainable for a solo entrepreneur .

### Key Competencies

  * **Business Strategy:** Translating qualitative pain points into a structured digital roadmap.
  * **Project Management:** Defining KPIs and deliverables within a strict timeline.

-----

## 6\. MagiCouture (Business Innovation)

**Tools:** Business Model Canvas, Prototyping

### Project Goal

To conceptualize a sustainable business model that addresses the environmental impact of fast fashion. We designed "MagiCouture," a platform connecting clients with local tailors for custom-made clothing .

### Methodology & Techniques

  * **Market Gap Analysis:** Identified that while consumers want sustainable options, current solutions (luxury/second-hand) lack personalization or affordability .
  * **Solution Design:** Propoesd a 3D modeling feature allowing users to visualize garments before production, reducing textile waste and ensuring inclusivity for all body types .
  * **Value Proposition:** Structured the service to act as a matchmaker, providing visibility to independent tailors while offering customers a "satisfaction or retouch" guarantee .

### Key Competencies

  * **Entrepreneurship:** Developing a viable business model from an initial problem statement.
  * **User-Centric Design:** Creating personas to tailor the service to specific market segments (e.g., eco-conscious professionals) .
