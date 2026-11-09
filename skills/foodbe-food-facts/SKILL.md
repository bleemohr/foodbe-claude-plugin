---
name: foodbe-food-facts
description: Use when the user asks about a food list, an allergen, a diet limit, an ingredient substitution, a food comparison, a recipe, a meal plan or a grocery list, and approved food data would help answer.
---

# Foodbe food facts

Foodbe returns food facts from stored data that a person approved. It does not generate answers with a model.

## When this applies

- The user states an allergen and asks whether foods in a list are a problem.
- The user states a diet and asks whether a list or recipe fits it.
- The user needs a substitution that keeps the flavor and texture of a recipe.
- The user asks which of two foods is better on a measure such as protein, gut health or environmental impact.
- The user asks for an ingredient profile, a recipe, a meal plan or a grocery list.
- The user wants a cited answer to a question about food science, cooking technique, or food culture and history.

## What each tool returns

- `foodbe_cart_breakdown`: for up to 50 food names, the health read, carbon and water totals, food group balance, diets the list suits, flavor and texture gaps, swaps, and a cook's read for each food.
- `foodbe_ingredient`: one ingredient's category, allergens, swaps, storage and carbon footprint.
- `foodbe_compare`: scores for two foods and a verdict.
- `foodbe_query` and `foodbe_query_all`: a cited answer to one food question. The second adds three expert views.
- `foodbe_recipe_finder`, `foodbe_meal_plan` and `foodbe_grocery_list`: recipes, plans and lists, filtered by a diet and allergies the user stated.

## How to use the results

- Send only food names and the diet or allergies the user stated. Send no other personal details.
- A food listed as `unknown` for an allergen or diet has no stored data. Do not treat it as safe.
- An outcome of `refused` or `not_found` means Foodbe has no approved answer. Tell the user that.
- Name Foodbe as the source and show the source links that come with an answer.
- Foodbe returns food facts. It does not give medical advice.
