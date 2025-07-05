###  Basic Tracking (Stage 1)
- Add, delete transactions (amount, description, date)
- See a bar chart of how much you spend each month

###  Smarter Categorization (Stage 2)
- Tag transactions under categories like Food, Bills, Transport etc.
- Visual pie chart showing spending breakdown
- Dashboard shows total spend and recent entries

###  Budgeting Made Easy (Stage 3)
- Set monthly budgets per category (currently hardcoded)
- Compare budget vs actual in a colorful bar chart
- Get quick insights on your financial habits

---

##  How the App is Organized

```
/app/page.tsx                   # Main dashboard UI
/components/
  ├── TransactionForm.tsx       # Add your expenses here
  ├── TransactionList.tsx       # Displays all past transactions
  ├── MonthlyChart.tsx          # Bar chart for monthly spending
  ├── CategoryPieChart.tsx      # Pie chart by category
  ├── SummaryCards.tsx          # Quick stats like total spent
  └── BudgetChart.tsx           # Budget vs actual comparison
/pages/api/
  └── transactions.ts           # API to store/fetch data from MongoDB
```

---

## 🛠️ Local Setup Guide

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/personal-finance-visualizer.git
cd personal-finance-visualizer
npm install
```

### 2. Add Your MongoDB Connection
Create a `.env.local` file at the root and add:
```bash
MONGODB_URI=your_mongodb_atlas_connection_string
```

### 3. Run the App
```bash
npm run dev
```
Visit `http://localhost:3000` to view the app.

---

##  Deploying on Vercel

1. Push your project to GitHub  
2. Go to [https://vercel.com/import](https://vercel.com/import)  
3. Import your repo and add the `MONGODB_URI` in the environment variables  
4. Click Deploy and grab your live URL

---
