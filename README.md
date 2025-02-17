# ETL Process for Shopping Website Data (Group Project TTTC3213)
This project demonstrates the ETL (Extract, Transform, Load) process using data scraped from the GoodRead website, focusing on product details such as Title,Author,Reviews and etc. It is completed as part of the TTTC3213 Group Assignment for the academic term, adhering to the guidelines provided.
#
## Project Overview
**Objective**
To extract, transform, and load book data from Goodreads and visualize insights for analysis.

**Group Members**
1. FADHLEE FAYYADH BIN MOHD RASDI(A195682) : Number of People Vote, Genre
2. NUR ALYSSA SOFEA BINTI EDRIAN (A195034) : Score, Ratings
3. NURQISTINA DAMIA BINTI SHAHRINE (A193964) : Title, Author
4. NUR SABRINA BINTI MOHD HILMAN RAJANG (A192047) : Date Published, No of Reviews

**Dataset**
- **Website**: [Goodread - Best Young Adult Books Collection](http://goodread)
- **Records**: 200 Books Scraped.

#

## ETL Breakdown

### 1. Extract (10 Points)

**Dataset Selection:**

- Chose the Goodreads website for its rich book data (e.g., ratings, reviews, genres, publication date).

- Verified that scraping this site is legal and ethical.

**Data Scraping:**

- Used Python libraries: BeautifulSoup, requests.

**Extracted attributes:**

- Book details: Title, Author, Score, Ratings, Number of People Voted, Genre, Date Publication, Number of Reviews.


**Record Count:**

- Successfully collected 200 book records with all required attributes.

### 2. Transform (10 Points)

**Data Cleaning:**

1. Standardization the Date Published: Converted Date format (eg. from **"First published June 26, 1997"** to **"1997-06-26"**.

2. Sorting: Arranged books in ascending order by **Title**.
3. Numerical Conversion: Extracted numeric values from ratings and removed non-numeric characters from review counts.

4. Removing Non-Numeric Characters: Ensures that the attribute contains only integers, removing any unwanted text at **Number of Reviews**.

**Data Visualisation:**
- **Before Cleaning**:
- **After Cleaning**:

  
### 3. Load (2 Points)
- The cleaned data is saved into a CSV file (raw_data.csv), which can be easily read by pandas or other tools.

### 4. Report (8 Points)
**Experience Documentation:**
1. A detailed project write-up is published on [Medium](https://medium.com/@a192047/scrape-and-perform-extraction-transformation-loading-etl-on-goodreads-3c29abaf688a).
2. The Medium article includes:
   - Code explanations.
   - Visualizations (before and after cleaning).
   - GitHub repository link to the project.

**Submission:**
- Shared the Medium link and cleaned .csv file on UKMFolio.

## Repository Structure

```
├── GROUPPROJECT_DATA_ENGINEERING.ipynb  # Main ETL process and code  
├── raw_data.csv                         # Raw scraped data  
├── cleaned_data.csv                     # Cleaned and processed data  
└── README.md                            # Project documentation  
```


## Setup Instructions
1. Clone the repository:

        git clone https://github.com/DataEngineering.git

        cd DataEngineering

2. Install dependencies:

        pip install -r requirements.txt

3. Run the ETL process:
   - Open GROUPPROJECT_DATA_ENGINEERING.ipynb in Jupyter Notebook.
   - Execute all cells to scrape, clean, and visualize data.
     
#

## Tools & Libraries
- Libraries: BeautifulSoup, requests, pandas, matplotlib
- Environment: Python 3.x, Jupyter Notebook
- Platform: Medium for documentation, GitHub for code hosting.

## Key Insights
- Scraped over 200 book records from the Goodreads website.
- Transformed raw data into a clean format suitable for analysis.


