# Training Data

* **data_train.csv** (~16MB, 36283 lines) is a text file (UTF-8) containing product features.  Each line in the file refers to a specific product.
  The features are presented in comma-separated values format:

  ```
  country,sku_id,title,category_lvl_1,category_lvl_2,category_lvl_3,short_description, price,product_type
  ```

  For example:

  ```
  my,NO037FAAA8CLZ2ANMY,RUDY Dress,Fashion,Women,Clothing,"<ul> <li>Short Sleeve</li> <li>3 Colours 8 Sizes</li> <li>Dress</li> </ul> ",33.0,local
  ```

* **clarity_train.labels** (~100KB, 36283 lines) is a text-file that contains ground-truth labels for the Clarity scoring.  Each line corresponds to the same product in data_train.csv.  The label has two possible values: 1 = clear, or 0 = not clear.  Distribution in this file: 94.3% are labeled 1, while 5.7% are labeled 0.

* **conciseness_train.labels** (~100KB, 36283 lines) is a text-file that contains ground-truth labels for the Conciseness scoring.  Each line corresponds to the same product in data_train.csv.  The label has two possible values: 1 = concise, or 0 = not concise.  Distribution in this file: 68.5% are labeled 1, while 31.7% are labeled 0.

# Validation Data

**data_valid.csv** (~5MB, 11838 lines) is a text-file (UTF-8) containing product features.  It has the same format to data_train.csv.

# Testing Data

**data_test.csv** (~5MB, 12674 lines) is a text-file (UTF-8) containing product features.  It has the same format to data_train.csv.
