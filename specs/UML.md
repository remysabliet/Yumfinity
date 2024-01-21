+------------------+        +-----------------+       +------------------+
|     Recipe       |        |   Ingredient    |       |     Ustensil     |
+------------------+        +-----------------+       +------------------+
| - recipeId: string|        | - ingredientId:  |       | - ustensilId: string|
| - title: string   |        |    string       |       | - name: string   |
| - description:    |        | - quantity: float|       +------------------+
|    string         |        | - imageUrl: string|
| - imageUrl: string|        | - unit: string   |
| - category: string|                                     
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
+------------------+

+------------------+        +------------------+
|      User        |        | UserCredentials  |
+------------------+        +------------------+
| - userId: string |        | - userId: string |
| - username: string|        | - password: string|
| - email: string   |                           
| - fullName: string|                           
+------------------+                           
