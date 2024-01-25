# Functional specifications

## 1 Purpose
The purpose of the Recipe Application is to provide users with a platform to discover, create, and share recipes. The application supports the management of recipes, ingredients, ustensils, and user interactions.

## 2 User Interaction
- User authentication is required to access recipes.
- A user can create/edit/delete their own recipes.
- A user can view their recipes as part of a special filter "My recipes," or view all recipes otherwise. By default, a user sees all recipes.
- Recipes are categorized (e.g., Beverage, Soup, etc.), and a category might have subcategories, such as Cocktail and Mocktail for beverages.
- Users can give a rating up to 5 stars to a recipe (1, 2, 3, 4, 5). When a user visits a recipe they've rated before, they can see their previous rating and cannot double-rate the same recipe.
- Users can search for recipes through an input search field using keywords. Keywords will be matched with a recipe title or tags assigned to them.

## 3 Recipe
- A recipe is a composition of:
- A list of ingredients along with their measure unit and quantity.
- A list of ustensils required to perform the recipe.
An ordered list of steps. Every step includes a description and could eventually include media like an image, a movie, or a voice recording.

## 4 Ingredient
- A default list of ingredients will be provided.
- If an Ingredient is not part of the list, a user will have the possibility to register a custom Ingredient.
- A list of pre-defined unit measures is available by default.

## 5 Rating System
- Users can give ratings to recipes on a scale of 1 to 5 stars.
- When revisiting a recipe, users can see their previous rating and cannot rate the same recipe again.
- A user has the option to delete one of their previous ratings or simply re-rate.

## 6 Search Functionality
- Users can search for recipes using keywords in the search field.
- Keywords are matched with recipe titles or tags.

## 7 Categories and Subcategories
- Recipes are categorized into main categories (e.g., Beverage, Soup).
- Main categories may have subcategories (e.g., Cocktail and Mocktail for beverages).

## 8 Customization
- Users can register custom ingredients not present in the default list.
- Users can register custom unit of measure not present in the default list.