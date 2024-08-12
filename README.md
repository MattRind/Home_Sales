# Home_Sales
- This repo contains one jupyter notebook and this Markdown file. 
- Summary of the analysis to determine key metrics about home sales data is included below: 
   - A query was run to determine the average price of a home per 'view' rating having an average home price greater than or equal to $350,000. From a temporary view of the dataset, the query took 0.989 seconds to run. The same query using cached data took 0.819 seconds to run. Running the original query after the dataset was partitioned by the "date_built" field as a formatted parquet took 1.356 seconds to run. One observation is that for all scenarios, the run time for the queries was relatively fast, possibly the benefits of using a Google server. Running the query was the fastest using the cached data (before creating a parquet). One possible reason the partitioned data took slightly longer (0.5 seconds) is that the query itself yielded a relatively small set of data, diminishing the advantage of partitioning.
- The data analyis was run in Google Colab. A jupyter notebook template was originally provided, which I followed for answering the questions in the Challenge. 
- All new code was written by me.
