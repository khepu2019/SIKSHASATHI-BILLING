# Sikshasathi — Shop Inventory, POS, Customer Ledger, Admin & Billing System

A complete, single-file ERP & Point-of-Sale (POS) web application built for **Sikshasathi** (Books, Stationery, Academic Supplies & General Store) with real-time Profit & Loss (P&L) analytics, Customer Ledger passbooks, Product Returns, Expense Vouchers, and Maker-Checker Admin Approval controls.

## ✨ Key Features

- **POS & Smart Billing Counter (`₹` INR)**
  - Fast product search by name, SKU, or category with barcode/Enter key support
  - Quantity units support (`Pcs`, `Kg`, `Gram`, `Ltr`, `ml`, `Pack`, `Box`, `Dozen`, `Set`, `Roll`, `Meter`) including decimal quantities
  - Per-item discount (`₹` or `%` with decimal support like `2.25%`) and overall bill discount (`₹` or `%`)
  - Optional Tax (VAT/GST `%`) toggle and Service Charge (`₹` or `%`)
  - Permanent, non-deletable **`CASH`** customer account (with Mobile Number auto-disabled when `CASH` is selected)
  - Live Customer Name & Mobile Number search dropdown (`Customer Name — Mobile No (Ledger Balance)`)
  - Print-ready Tax Invoices in **A4 Standard** and **Thermal 80mm Receipt** formats

- **Inventory & Stock Master**
  - Automatic stock deduction on billing and automatic restocking on product returns
  - Stock valuation (Purchase Cost vs. Retail Value) and Low/Out-of-Stock alerts
  - Product Category management

- **Customer Ledger Passbook System**
  - Auto-creates customer ledgers from the POS counter or Customer Directory
  - Tracks total billed, total paid, current due balance, and advance deposits
  - One-click **+ Add to Bill** from any customer ledger

- **Product Returns & Refunds**
  - Invoice-linked item returns with automatic inventory restock and customer ledger/due adjustment

- **Real-Time Profit & Loss (P&L) Analytics**
  - Live per-bill and overall P&L calculation:
    `Net Profit = ∑(Selling Price − Last Purchase Price) − Total Discounts + Service Charges`

- **Sikshasathi Admin Control Panel & Maker-Checker Approval Queue**
  - Two operator roles with password authentication:
    - **Sales Counter** (Default Password: `1234`)
    - **Sikshasathi Admin** (Default Password: `admin123`)
  - Admin Approval Queue for product additions/edits/deletions, customer deletions, category changes, stock adjustments, and shop expense vouchers
  - Shop Expense Voucher Book with custom Expense Category management
  - Timestamped Security & Activity Audit Log
  - Full JSON Database Backup & Restore (`localStorage`)

## 🚀 How to Deploy on GitHub & GitHub Pages

### Option 1: Upload Directly via GitHub Web Interface (No Coding Required)
1. Sign in to [GitHub](https://github.com) and click the **`+`** icon in the top-right corner → **New repository**.
2. Enter a repository name (e.g., `sikshasathi-pos-erp`), select **Public** (or **Private**), and click **Create repository**.
3. Click **uploading an existing file** on the repository setup page.
4. Drag and drop `index.html` and `README.md` (extracted from the ZIP file) into the browser window.
5. Click **Commit changes**.
6. **Enable Live Website (GitHub Pages)**:
   - Go to **Settings** → **Pages** (in the left sidebar).
   - Under **Build and deployment** → **Branch**, select `main` (or `master`) and `/ (root)`, then click **Save**.
   - In 1–2 minutes, your live POS app will be accessible at `https://<your-github-username>.github.io/sikshasathi-pos-erp/`.

### Option 2: Upload via Git CLI (Terminal / Command Prompt)
```bash
git init
git add index.html README.md .gitignore LICENSE
git commit -m "Initial commit: Sikshasathi ERP & POS System"
git branch -M main
git remote add origin https://github.com/<your-username>/sikshasathi-pos-erp.git
git push -u origin main
```
