# Level: Easy

## Deliverables
You are building an app for a national bakery chain
- your models are bakeries, desserts, ingredients
  - a bakery has many desserts
  - a dessert belongs to a bakery
  - a dessert has many ingredients
  - an ingredient belongs to a dessert
    - every ingredient has a calorie count
Write out the relationships using has_many, belongs_to and has_many_through. Create the necessary methods to connect these classes.



#### Ingredients
  - #dessert
    - should return a dessert object for that ingredient
  - #bakery
    - should return the bakery object for the bakery that uses that ingredient
  - .all
    - should return an array of all ingredients
  - .find_all_by_name(ingredient)
    - should take a string argument return an array of all ingredients that include that string in their name
      - .find_all_by_name('chocolate') might return ['chocolate sprinkles', 'chocolate mousse', 'chocolate']
      - make sure you aren't just looking for exact matches (like 'chocolate' == 'chocolate')
