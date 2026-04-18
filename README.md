# 📊 SEM A/B Test Analyzer (Frontend)

**Live Demo:** [https://sem-analyzer-ui.vercel.app](https://sem-analyzer-ui.vercel.app)  
**Backend API Repository:** [https://github.com/thit2003/sem-analyzer-api](https://github.com/thit2003/sem-analyzer-api)

## Overview
This is the frontend client for the SEM A/B Test Analyzer, a MarTech dashboard designed to automate the statistical analysis of Google Ads campaigns. 

Marketing teams often spend hours manually calculating Click-Through Rates (CTR), Conversion Rates (CVR), and running statistical significance tests in spreadsheets. This React application allows users to upload a raw Google Ads CSV export and instantly visualizes the winning ad variation based on a backend Z-Test algorithm.  

## 🚀 Features
* **Drag-and-Drop Interface:** Seamlessly accept `.csv` file uploads.
* **Instant Visualization:** Renders interactive bar charts comparing ad performance using Recharts.
* **Business Logic Display:** Clearly highlights the "Winning Ad" and displays the P-Value, indicating if the results meet the 95% industry standard for statistical significance.
* **Responsive Design:** Clean, modern UI built for both desktop and data-heavy dashboard views.

## Sample Data
To quickly try the live demo, upload one of the sample CSV files in `mock_csv/`.  
If you’d like to generate a custom dataset, run `mock_csv/generate_mock_data.py` and adjust parameters such as the output filename and the number of days.

```bash
python mock_csv/generate_mock_data.py
```

## 💻 Tech Stack
* **Framework:** React.js (Bootstrapped with Vite for optimal performance)
* **Data Visualization:** Recharts
* **Icons:** Lucide React
* **Deployment:** Vercel

## 🛠️ How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/thit2003/sem-analyzer-ui.git
   cd sem-analyzer-ui
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. **Connect the Backend:**
   Ensure the FastAPI backend is running locally on port `8000`. By default, this frontend is configured to point to the live deployed API, but you can change the fetch URL in `src/App.jsx` to `http://127.0.0.1:8000[...]
