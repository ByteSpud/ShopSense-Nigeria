# ShopSense Nigeria — Product Sales Tracker

**Python Capstone Assignment — 10Alytics Data Engineering Programme**

## About the Project

ShopSense is a small but growing phone accessories shop on Lagos Island. The store owner, Amara, has been tracking her products in a notebook, but it's getting too slow and she keeps missing restock warnings.

This project is a simple Python script that helps Amara by:

- Showing her which products are **HOT**, **STEADY**, or **SLOW** sellers
- Calculating total revenue and stock value
- Flagging products that need restocking before she runs out

## Role

Built as a **Junior Data Engineer** exercise: writing Amara's Python script from scratch so it runs top to bottom with no errors and prints a clean, formatted report.

## Data Structure

Each product record includes:

| Field | Type | Description |
|---|---|---|
| `name` | `str` | Product name |
| `price` | `float` | Selling price |
| `units_sold` | `int` | Units sold this week |
| `stock_left` | `int` | Units remaining |
| `is_featured` | `bool` | On promotion? |
| `category` | `str` | Product type |

## What the Script Does

The notebook is broken into four tasks:

1. **Define product records** — A list of 7 product dictionaries (6 provided, 1 added), with type verification for `price` (float) and `units_sold` (int).
2. **Classify products** — `classify_product()` returns a seller status based on units sold:
   - `HOT` — units_sold ≥ 30
   - `STEADY` — 15 ≤ units_sold < 30
   - `SLOW` — units_sold < 15
3. **Weekly shop report** — Loops through all products, classifies each, and prints a clean formatted report.
4. **Business insights** — Computes three key insights:
   - Best seller (highest units sold)
   - Total stock value (price × stock_left, summed across all products)
   - Restock alert (products with stock_left < 5)

## Files

- `ShopSense_Capstone_GH.ipynb` — the full Jupyter notebook containing the solution

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/ByteSpud/ShopSense-Nigeria.git
   cd ShopSense-Nigeria
   ```
2. Open `ShopSense_Capstone_GH.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
3. Run all cells top to bottom.

## Program Info

- **Programme:** Data Engineering
- **Assignment:** Python Capstone — ShopSense Nigeria
