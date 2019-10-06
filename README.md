# image_color_palette_clustering

Using Google's Vision API we can convert image files into numeric RGB values and engineer images into truly accurate color features for use in further analysis or data science products.

![Image of Architecture](https://raw.githubusercontent.com/alanjbates/image_color_palette_clustering/master/readme_images/vision_api_flow.png)


## image_color_palette.ipynb

First I used this notebook to do some data wrangling, call the Google Vision API, and to build an Image Color Palette in BigQuery.

This notebook uses the the Google Vision API to get Image Properties from web hosted images. Specifically it returns the Color Palette of the image in numeric RGB values. These Numeric Values can be used as input into other data products.

Step 1: Get list of image URls
Step 2: Scrape images from web
Step 3: Load image in to RAM
Step 4: Process Image with Google Vision API Image Properties method
Step 5: Flatten Response JSON into dataframe
Step 6: Load results to BigQuery


## color_family_clustering.ipynb

This is an example of how this numeric RGB data can be used to build data features that can be used as input into other data products.

