# 🍽️ Flutter Restaurant POS System

A full-featured restaurant **Point of Sale system** built with Flutter. Designed for real-world use in dine-in or takeaway restaurants. It covers everything from table-based sales to editable sale history and detailed reports.

---

## 📲 Demo Flow – Step-by-Step

### 🛡️ 0️⃣ Login
- Start by logging into the system with a valid username and password.
- Ensures only authorized staff can access the POS.
- After login, you'll be redirected to the Home screen.

> ![Step 0: Login](screenshots/step_0_login.png)

---

### 1️⃣ Add Table Number
- Start a sale by entering the table number.
- Prevents anonymous orders and links sale to a location.

> ![Step 1: Enter Table Number](screenshots/step_1_table_number.png)

---

### 2️⃣ Add Menu & Products
- Select category, menu, and products.
- Products can have quantity, taste level, and optional notes.
- Items are added to a live cart.

> ![Step 2: Add Products](screenshots/step_2_add_products.png)

---

### 3️⃣ Choose Payment Method
- After confirming the cart, choose a payment type: `Cash`, `Card`, or `Other`.

> ![Step 3: Choose Payment](screenshots/step_3_payment.png)

---

### 4️⃣ Dine-In or Parcel Dialog
- A dialog appears:
  - Choose: **Dine-In** or **Parcel**
  - Enter: Remarks (optional)
  - Choose: How many **prawn** and **octopus** were selected (optional)

> ![Step 4: Dine-in Dialog](screenshots/step_4_dinein_parcel_dialog.png)

---

### 5️⃣ Checkout Page
- See final sale summary:
  - Table number
  - Products, quantity, and total
  - Tax and discount breakdown
  - Ask: "Do you want to print slip?"
- Press `Checkout` to confirm the sale.

> ![Step 5: Checkout](screenshots/step_5_checkout.png)

---

### 6️⃣ Sale Success
- Show success dialog or toast.
- Auto-navigate back to Home.

> ![Step 6: Success](screenshots/step_6_success.png)

---

### 7️⃣ View Sale History
- Go to the **History** tab.
- See all past transactions listed by date and time.

> ![Step 7: History List](screenshots/step_7_history_list.png)

---

### 8️⃣ View History Detail
- Tap a history item to view its full detail:
  - Items sold
  - Table number
  - Payment method
  - Remarks
  - Parcel/Dine-in

> ![Step 8: History Detail](screenshots/step_8_history_detail.png)

---

### 9️⃣ Edit Sale History
- Tap `Edit` to:
  - Update products
  - Change remarks or quantity
  - Modify octopus/prawn counts

> ![Step 9: Edit History](screenshots/step_9_edit.png)

---

### 🔟 Edit History Success
- Save changes and confirm update.
- Sale updates reflected immediately in history and reports.

> ![Step 10: Edit Success](screenshots/step_10_edit_success.png)

---

### 🔢 View Sale Reports
- Go to the **Reports** tab.
- Filter by:
  - 🗓️ Daily
  - 📅 Weekly
  - 📈 Monthly
- View total sales, tax, discounts, and net revenue.

> ![Step 11: Reports](screenshots/step_11_reports.png)

---

## 🧱 Features Recap

- 🔐 Secure Login
- 📦 Product/Menu/Category CRUD
- 🍛 Taste Level & Notes
- 💳 Multiple Payment Methods
- 🧾 Receipt/Slip Printing
- 🕑 Sale History + Edit
- 📊 Sales Reports with Filtering
- ✅ Clean Architecture + BLoC

---

## 🛠️ Tech Stack

- Flutter 3.x
- flutter_bloc
- SQLite / Supabase / Laravel backend
- esc_pos_printer / bluetooth_print
- fl_chart for reporting

---

## 📦 Setup

```bash
git clone https://github.com/yourusername/flutter-pos-restaurant.git
cd flutter-pos-restaurant
flutter pub get
flutter run
