+------------------+        +-----------------+       +------------------+
|     Recipe       |        |   Ingredient    |       |     Ustensil     |
+------------------+        +-----------------+       +------------------+
| - recipeId: string|        | - ingredientId:  |       | - ustensilId: string|
| - title: string   |        |    string       |       | - name: string   |
| - description:    |        | - quantity: float|       +------------------+
|    string         |        | - imageUrl: string|
| - imageUrl: string|        | - unit: string   |
| - category: RecipeCategory |                                     
| - tags: string[]  |                           
| - rating: float   |                                    
+------------------+                                      
       |                           |                      |
       |                           |                      |
       |                           |                      |
       |                           |                      |
       |                           |                      |
       v                           v                      v
+------------------+    +------------------+   +------------------+
|    RecipeStep    |    | IngredientRecipe|   | UstensilRecipe   |
+------------------+    +------------------+   +------------------+
| - stepId: string |    | - ingredientId:  |   | - ustensilId: string|
| - description:    |    |    string       |   | - recipeId: string|
|    string         |    | - quantity: float|   +------------------+
| - imageUrl: string|    | - unit: string   |
| - videoUrl: string|    +------------------+
| - createdBy: User |      // CreatedBy relation                   
+------------------+      

+------------------+        +------------------+
|      User        |        | UserCredentials  |
+------------------+        +------------------+
| - userId: string |        | - userId: string |
| - username: string|        | - password: string|
| - email: string   |                           
| - fullName: string|                           
+------------------+       

+------------------------+      +---------------------+
|      UserRating       |      |   UserDefinedIngredient  |
+------------------------+      +---------------------+
| - userRatingId: string|      | - userIngredientId: string|
| - userId: string      |<-----| - userId: string    |
| - recipeId: string    |      | - name: string      |
| - rating: float        |      | - ingredientId: string |  // Foreign Key
+------------------------+      +---------------------+

+-----------------+         +------------------------+
|   Ingredient    |         |  MeasurementUnit       |
+-----------------+         +------------------------+
| - ingredientId  |         | - unitId: string       |
| - name: string  |         | - name: string         |
| - ... other fields |      +------------------------+
| - unitId: string |<------| - abbreviation: string |
+-----------------+         +------------------------+
