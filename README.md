# food-recipes-dataset

The dataset used in this study consists of 866 recipes obtained from two sources:

- 304 recipes from The Meal DB, a free recipe API.
- 562 recipes collected via web scraping from Food.com.

##　Data Type and Composition

The dataset contains the following attributes:

- id: Unique identifier for each recipe.
- name: The title of the recipe.
- country: The country to which the recipe comes from.
- instructions: Step-by-step directions for preparing the dish.
- ingredients: A list of ingredients used in the recipe.
- region (target variable): The continent to which the recipe belongs.

In this dataset, only the id attribute is represented as an integer, while all other attributes are stored as text.

An example data entry is as follows:

52855,Banana Pancakes,American,"In a bowl, mash the banana with a fork until it resembles a thick purée. Stir in the eggs, baking powder and vanilla. Heat a large non-stick frying pan or pancake pan over a medium heat and brush with half the oil. Using half the batter, spoon two pancakes into the pan, cook for 1-2 mins each side, then tip onto a plate. Repeat the process with the remaining oil and batter. Top the pancakes with the pecans and raspberries.",1 large Banana; 2 medium Eggs; pinch Baking Powder; spinkling Vanilla Extract; 1 tsp Oil; 25g Pecan Nuts; 125g Raspberries,America

##　Data Collection

The dataset for this study comprises 866 recipes, gathered from two distinct sources: an API and web scraping.

###　From API

Using the API, I traversed through all available countries and retrieved their respective recipe IDs. These IDs were then used to query detailed information about each recipe. The retrieved data was filtered to obtain relevant attributes, such as recipe name, ingredients, and instructions, which were essential for further analysis.

###　From Web Scraping

For additional data, I employed web scraping techniques to collect recipe information from Food.com. I specifically focused on recipes categorized under different cuisines. The web crawler systematically navigated through each cuisine category, collecting all available recipes and their associated details. Similar to the API method, the data was processed to extract attributes such as ingredients, cooking instructions, and so on.
