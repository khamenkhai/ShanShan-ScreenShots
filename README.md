# 🍽️ Flutter POS Restaurant App

A powerful and modern **Point of Sale (POS)** system built with Flutter, designed specifically for restaurants and cafes. This app includes a sleek **sale system**, comprehensive **admin control panel**, and advanced **reporting** tools.

---

## 🚀 Features

### 🛒 Sales System
- Quick product selection by category or menu
- Add multiple items with quantity and custom taste levels
- Tax and discount handling
- Custom notes on items
- Voucher/slip preview and printing
- Edit slip before checkout
- Split payments (cash, card, etc.)
- Refund support

### 🧑‍💼 Admin Control Panel
- CRUD for:
  - Products
  - Categories
  - Menus
  - Taste Levels (e.g., spicy levels, cooking preferences)
- Upload product images
- Assign products to multiple categories/menus
- Enable/disable items for sale

### 📊 Sales Report & History
- View daily, weekly, monthly, and custom reports
- Total sales, profit, tax, and discount breakdown
- Export reports (CSV/PDF)
- Sale history with filtering by date, user, or item
- Edit past sale records with permission
- Edit slips and reprint

---

## 🧱 Architecture

This app follows **MVC** using BLoC for state management:


![image alt](https://github.com/khamenkhai/ShanShan-ScreenShots/blob/main/screenshots/Screenshot_1741274492.png?raw=true)


---

## 🛠️ Tech Stack

- Flutter 3.x
- BLoC (flutter_bloc)
- SQLite / Supabase (optional)
- `flutter_slidable`, `file_picker`, `fl_chart`, `flutter_bloc`
- Receipt printing: `esc_pos_printer`, `bluetooth_print`

---

## 🚀 How to Use

### 1. 🧾 Start a New Sale
- Navigate to the **Sale** screen.
- Select a product.
- Set quantity, notes, and taste preferences.
- Click `Add to Order`.

> ![Start Sale](screenshots/start_sale.png)

---

### 2. 🧮 Review & Checkout
- Edit items, apply discount, tax, or voucher.
- Choose payment method and complete the sale.

> ![Checkout](screenshots/checkout.png)

---

### 3. 🧑‍💼 Manage Products
- Go to the **Admin > Products** tab.
- Add/Edit/Delete products.
- Upload images and assign to categories.

> ![Product Admin](screenshots/product_admin.png)

---

### 4. 🍽️ Manage Menus & Taste Levels
- Create new menus (e.g., Drinks, Mains).
- Add taste levels (e.g., Mild, Spicy, Extra Spicy).
- Assign to products.

> ![Menus and Taste](screenshots/menu_taste.png)

---

### 5. 📅 View Reports
- Go to the **Reports** tab.
- Filter by day, week, month.
- View revenue, discounts, and net sales.
- Export or share.

> ![Reports](screenshots/report_view.png)

---

### 6. 📝 Edit Sale History & Slip
- View **History**
- Tap any sale to edit or reprint the slip.

> ![Edit Slip](screenshots/edit_slip.png)

---

## 📦 Installation

### Requirements
- Flutter SDK
- VS Code / Android Studio
- Supabase or Laravel Backend (optional)

### Setup

```bash
git clone https://github.com/yourusername/flutter-pos-restaurant.git
cd flutter-pos-restaurant
flutter pub get
flutter run

