# PulseFlow — Freelancer Cash Flow & Payment Alerts Dashboard

A high-performance, zero-dependency financial management dashboard built specifically for freelancers, consultants, and independent agencies to monitor cash flow runway, automate invoice reminders, and eliminate late payment anxiety.

---

## 🌟 Key Features

1. **Cash Flow Trajectory & 90-Day Forecast**:
   - Interactive SVG line/area visualization comparing **actual bank balance** vs **projected runway**.
   - Safety buffer floor line (default $5,000 threshold) with low balance warnings.
   - Dynamic runway calculation in months based on live liquid cash and current burn rate.

2. **Real-Time Payment Alerts & Chaser Center**:
   - Automated detection of **delinquent invoices** (past due date) and **upcoming milestones** (due in < 7 days).
   - **1-Click Chaser System**: Pre-written, customizable reminder templates:
     - 😊 Gentle / Early Ping
     - ⚖️ Standard Accounts Payable Follow-Up
     - 🚨 Urgent Overdue Notice with wire remittal request
   - One-click copy-to-clipboard and reminder counter tracking.

3. **"What-If" Runway Simulator**:
   - Interactive sliders to stress-test your freelance business:
     - Client payment delay simulation (0 to 60 days late).
     - Monthly burn rate adjustments ($2k to $8k/mo).
     - Safety reserve buffer adjustments.
   - Instant calculation of your projected **Zero-Cash Date** and risk level.

4. **Tax Safe-Harbor Reserve**:
   - Automated 25% tax withholding estimation so you never accidentally spend money owed for quarterly estimated taxes.
   - Clear distinction between **Total Liquid Balance** and **Safe-to-Spend Balance**.

5. **Invoice & Client Health Management**:
   - Full lifecycle management: Draft &rarr; Pending &rarr; Overdue &rarr; Paid.
   - Fast "+ New Invoice" creation with Net 7 / Net 14 / Net 30 terms calculation.
   - Client concentration analysis (warns when a single client accounts for >35% of total portfolio revenue).
   - CSV export for tax season and bookkeeping.
   - `localStorage` persistence with one-click demo data reset.

---

## 🚀 How to Run

### Method 1: Python Local Server (Recommended)
Run the provided Python server:
```powershell
python server.py
```
Then visit `http://localhost:8080/index.html` in your browser.

### Method 2: Direct Open in Browser
Double-click `index.html` in Windows Explorer or open it directly in Chrome, Edge, or Firefox. No build tools or node_modules required!

---

## 🛠️ Tech Stack
- Modern HTML5, Semantic CSS, JavaScript (ES6+)
- Tailwind CSS (via official gstatic script)
- Crisp SVG vector graphics for charts (zero third-party charting libraries needed)
- LocalStorage state management
