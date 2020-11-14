# Perform an analysis of customer behavior within e-commerce store
- The target of this research analysis is to manipulate and interpret meaningful patterns in the given data that could give us the ability to make precise, data-driven sales management decisions. Hence maximize the sales capacity, and also meet customer need.
## Data to analyze 
- Behavior data for 2 month (from October to November 2019 ) of a large multi-category online store (13.67 GB)
#### Because of the large dataset, Dask dataframes is used to read and write the csv data in Parquet formats, to facilitate computation speed and memory.
## Dataset structure
Each row in the file represents an event. All events are related to products and users. There are different types of events.
- event_time
  - Time when event happened at (in UTC).
- event_type
  - view - a user viewed a product
  - cart - a user added a product to shopping cart
  - removefromcart - a user removed a product from shopping cart
  - purchase - a user purchased a product
- product_id
  - ID of a product
- category_id
  - Product's category ID
- category_code
  - Product's category taxonomy (code name)
- brand
  - Downcased string of brand name. Can be missed.
- price
  - Float price of a product.
- user_id
  - Permanent user ID.
- user_session
  - Temporary user's session ID. Same for each user's session. Changed every time user come back to online store from a long pause.
## Script descriptions
- ADM-HW2.ipynb
  - Jupyter notebook script that contains the solutions to all the research questions
  
