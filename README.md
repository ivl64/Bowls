# 🥗 Bowl Meal Planner
 
A self-contained, offline-first mobile web app for planning and executing a high-protein bowl diet. One HTML file hosted on GitHub pages, can be shared via Telegram, save to phone's home screen, or host anywhere.
 
Built for German retail (REWE links included). Interface in Russian with a one-tap switch to German.
 
---
 
## Features
 
- **Weekly schedule** — 7 day cards with 4 meals each (breakfast, lunch, snack, dinner)
- **One grain per day** — single batch cooked each morning, split across 3 bowl meals
- **One vegetable set per day** — one leafy green + two vegetables used across all meals
- **Training-aware snack** — post-workout shake shown only on training days (Wed + Sun); rest days marked as such
- **Batch cook cards** — Sunday and Wednesday prep sessions with exact weights and oven times
- **Shopping list** — filterable by day (Saturday full shop / Wednesday greens top-up), REWE links, checkboxes with localStorage persistence
- **Bilingual** — Russian / German toggle, persisted across sessions
- **Dark mode** — follows system preference automatically
- **Standalone** — single `.html` file, no dependencies, works offline
---
 
## Usage
 
1. Download `index.html`
2. Open in any browser — or share the file directly via Telegram / WhatsApp
3. On iPhone: Safari → Share → Add to Home Screen
4. On Android: Chrome → ⋮ → Add to Home Screen
No account, no internet required after the first open.

Hosted on GH: https://ivl64.github.io/Bowls/

---
 
## Weekly Structure
 
### Shopping
 
| Day | What |
|---|---|
| **Saturday** | Full shop — grains, all proteins (frozen + fresh), dairy, vegetables, snack items |
| **Wednesday** | Top-up — fresh spinach (Friday), rucola (Sunday), avocado ×3 |
 
### Cooking
 
| Session | When | What |
|---|---|---|
| **Batch 1** | Sunday ~1 h | Chicken breast 120g (Mon lunch) · Turkey breast 300g (Tue + Wed lunch) · Oil-based dressings D1 D2 D3 D7 |
| **Batch 2** | Wednesday ~1 h | Chicken breast 245g (Thu + Fri lunch) · Chicken thighs 265g (Sat dinner) · Salmon 130g (Thu breakfast) · Yogurt dressings D4 D5 D6 D8 |
| **Daily grain** | Each morning ~15–30 min | One grain type cooked fresh, portioned into 3 containers |
| **Daily seafood** | Each evening ~10–15 min | Thawed overnight, cooked fresh |
 
---
 
## Nutrition Framework
 
### Daily targets
 
| Scenario | Protein | Carbs | Fat |
|---|---|---|---|
| Training day (Wed + Sun) | 170 g | 200 g | 100 g |
| Rest day (Mon Tue Thu Fri Sat) | 140 g | 160 g | 85 g |
 
### Per-meal breakdown
 
| Meal | Protein | Carbs | Fat | Notes |
|---|---|---|---|---|
| Breakfast | 40 g | 60 g | 25 g | Grain portion + protein source + light dressing |
| Lunch | 45 g | 70 g | 30 g | Pre-cooked protein from batch session |
| Post-workout snack | 30 g | 40 g | 15 g | Protein shake + milk + banana + peanut butter 10g |
| Dinner | 55 g | 30 g | 30 g | Smaller grain portion, higher protein, fresh-cooked seafood |
 
Snack is included **only on training days**. On rest days the daily total is 3 meals only.
 
### Protein sources
 
Protein is rotated across the week to avoid monotony and cover different amino acid profiles:
 
| Source | Type | g protein / 100g |
|---|---|---|
| Graved Lachs (gravlax) | Fatty fish | 18 |
| Salmon fillet | Fatty fish | 20 |
| Tuna (canned, own juice) | Lean fish | 25 |
| Tuna steak | Lean fish | 23 |
| Cod fillet | Lean fish | 18 |
| Shrimp | Seafood | 19 |
| Squid rings | Seafood | 16 |
| Chicken breast | Poultry | 23 |
| Turkey breast | Poultry | 22 |
| Chicken thighs | Poultry | 18 |
| Veal (fillet) | Red meat | 21 |
 
### Fat additions
 
Fat targets are met through dressing + toppings. The type depends on the protein source:
 
| Protein type | Fat addition |
|---|---|
| **Fatty** (gravlax, salmon, chicken thighs) | Olive oil 5g + nuts 10g |
| **Lean — breakfast** | Avocado 50g + olive oil 8g + nuts 15g |
| **Lean — lunch / dinner** | Avocado 75g + olive oil 10g + nuts 10–15g |
 
### Carbohydrate sources
 
One grain per day, cooked as a single batch and split across meals:
 
| Grain | Carbs per 100g dry | Weekly use |
|---|---|---|
| Quinoa | 60 g | Monday + Friday |
| Brown rice | 74 g | Tuesday |
| Buckwheat | 70 g | Wednesday + Sunday |
| Bulgur | 57 g | Thursday |
| Couscous | 73 g | Saturday |
 
### Vegetables
 
Each day uses one leafy green + two vegetables across all three bowl meals:
 
| Day | Green | Veg 1 | Veg 2 |
|---|---|---|---|
| Monday | Spinach | Cucumber | Tomato |
| Tuesday | Rucola | Carrot | Radish |
| Wednesday | Feldsalat | Fennel | Celery |
| Thursday | Romana | Carrot | Bell pepper |
| Friday | Spinach | Tomato | Cucumber |
| Saturday | Iceberg | Radish | Bell pepper |
| Sunday | Rucola | Fennel | Carrot |
 
Hardy vegetables (carrot, bell pepper, radish, fennel, celery, cucumber) are prepped once on Saturday. Leafy greens are bought fresh: Saturday batch covers Mon–Thu, Wednesday top-up covers Fri and Sun.
 
### Dressings (D1–D8)
 
Eight dressings rotate across the week — four oil-based (prepared Sunday, last the full week) and four yogurt-based (prepared Wednesday, last 3–4 days):
 
| | Recipe |
|---|---|
| D1 | Olive oil 15g · sesame oil 5g · soy sauce 5g · garlic powder |
| D2 | Olive oil 15g · balsamic vinegar 10g · oregano |
| D3 | Olive oil 15g · lemon juice 10g · dill |
| D4 | Greek yogurt 50g · tomato paste 10g · garlic · paprika |
| D5 | Greek yogurt 50g · mustard 5g · lemon juice |
| D6 | Tahini 20g · lemon juice 10g · garlic · water |
| D7 | Olive oil 15g · parsley · dill · coriander · garlic |
| D8 | Greek yogurt 50g · cucumber 30g · dill · garlic |
 
---
 
## Notes
 
- All frozen proteins are purchased on Saturday and thawed overnight in the fridge as needed. Each day card includes a thaw reminder.
- Veal (Sunday lunch) is cooked fresh — it takes ~20 minutes and is the only Sunday cooking beyond the shake.
- Avocado ripeness management: buy 2 ripe + 2 firm on Saturday for Mon–Thu; buy 3 on Wednesday for Fri–Sun.
- Protein powder brand is not specified — any whey or blend with ~80g protein per 100g works.
- Toppings (nuts, seeds) are interchangeable. The shopping list covers a full variety; use whatever matches the dressing.
 
