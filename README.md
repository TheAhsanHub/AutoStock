#  AutoStock

**A car dealership inventory and sales management system, built in Python with a Tkinter GUI.**

AutoStock helps a car dealership manage its stock and sales digitally. Customers can browse, search and buy cars, while admins manage the inventory and track every sale. All data is saved to CSV files, so records persist between sessions with no database setup.

## Features

**User panel**
- Browse all cars in a sortable table
- Search by brand, model, year, cost or colour, or sort by any column
- Buy a car by entering customer and salesperson names. The car is marked **Sold** and a sale record is created automatically
- Prevents buying a car that's already sold

**Admin panel**
- Add, update and delete cars (click a row to auto-fill the edit form)
- View the full inventory
- View sales history: date, unique sales ID, brand, customer, price and salesperson

##  Tech stack

- **Python 3**
- **Tkinter / ttk** for the GUI (tabbed `Notebook`, `Treeview` tables, forms and dialogs)
- **CSV** files for persistent storage (`cars.csv`, `sales.csv`)
- Modular design: separate functions for reading, writing and logging sales, and the GUI wrapped in a `CarManagerApp` class

## Getting started

Tkinter comes with Python, so there's nothing to install.

    git clone https://github.com/TheAhsanHub/car-inventory-system.git
    cd car-inventory-system
    python "Car inventory.py"

On first run, the app creates `cars.csv` and `sales.csv` automatically. Choose **Admin Panel** to add some cars, then switch to the **User** tab to search and buy.

## Data format

| File | Columns |
|---|---|
| `cars.csv` | Brand, Model, Year, Cost, Shade, Status |
| `sales.csv` | Date, SalesID, Brand, CustomerName, PriceSold, Salesperson |

## 🔭 Future improvements

- Admin login with password protection
- Move storage to SQLite for faster search and safer updates
- Input validation for year and price fields
- Sales reports and charts (e.g. revenue per month)

## Author

**Ahsan**, BSc (Hons) Computer Science, Cardiff Metropolitan University
