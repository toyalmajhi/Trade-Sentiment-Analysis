# 🧠 Trade Sentiment Analysis

This project explores the relationship between **market sentiment** and **trader performance** using data from the **Fear & Greed Index** and **Historical trading dataset**. The goal is to uncover insights that can support smarter trading strategies.

---

## 📊 Project Objectives

- Analyze how market sentiment (Fear or Greed) affects trading outcomes.
- Calculate metrics like total profit/loss, win rate, and trade volume under different sentiment conditions.
- Identify behavioral patterns among traders during different sentiment phases.

---

## 📁 Datasets Used

1. **Fear & Greed Index**  
   - Columns: `timestamp`, `Date`, `Classification`, `date` (Fear or Greed)

2. **Historical Trader Data**  
   - Columns: `Account`, `Coin`, `Execution Price`, `Size Tokens`, `Size USD`, `Closed PnL`, `Timestamp IST`, `Direction`, `Transaction Hash`, `Order ID`, etc

---

## 🛠️ Tools & Libraries

- Python
- Pandas
- Matplotlib / Seaborn
- Jupyter Notebook

---

## 🔍 Key Steps

1. **Data Cleaning**
   - Parsed timestamps and standardized column names
   - Converted PnL values and sizes to numeric types

2. **Data Integration**
   - Merged Fear and Greed Index data with Historical Trader data by date

3. **Feature Engineering**
   - Created a `Profit` flag based on `Closed PnL > 0`

4. **Analysis**
   - Grouped results by `account` and `classification`
   - Compared average profit, average pnl under sentiment such as fear and greed (classification column)
   - Sorted top 10 traders from the data

5. **Visualization**
   - Sentiment-wise distribution of trades and profits
   - Top profitable accounts during Fear vs. Greed phases
     
---

## 📈 Insights

- Traders tend to be **more profitable during Greed** periods.
- Some accounts consistently perform well regardless of sentiment, indicating strategy-driven success.
- Larger position sizes are often taken during Greed, correlating with market optimism.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/toyalmajhi/trade-sentiment-analysis.git
   ```

2. Navigate to the folder:
   ```bash
   cd trade-sentiment-analysis
   ```

3. Run the Jupyter notebook:
   ```bash
   jupyter notebook
   ```

---

## 📌 Future Improvements

- Include real-time sentiment analysis via APIs
- Apply machine learning to predict trade outcomes based on sentiment
