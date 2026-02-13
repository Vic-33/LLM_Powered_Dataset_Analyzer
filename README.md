# [LLM Powered Dataset Analyzer](https://tds-project-2-j9sz.onrender.com/)

An **LLM-powered data analytics platform** that allows users to upload datasets and ask natural-language questions to generate automated insights and visualizations.

This project combines **FastAPI, LangChain, and Google Gemini** to interpret dataset patterns and answer queries with statistically supported explanations — reducing manual effort in exploratory data analysis.

---

## Features

-  Upload datasets for instant analysis
-  Ask natural-language questions about your data
-  Automated charts and visualizations
-  LLM-powered statistical insights
-  FastAPI backend for efficient API performance
-  Structured summaries for quick understanding
-  Reduced manual exploratory data analysis time

---

## Tech Stack

- **Backend:** FastAPI
- **LLM Integration:** LangChain + Google Gemini
- **Data Processing:** Python (Pandas, NumPy)
- **Visualization:** Matplotlib / Seaborn / Plotly *(update based on your actual stack)*
- **API Communication:** REST

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Vic-33/LLM_Powered_Dataset_Analyzer.git
cd LLM_Powered_Dataset_Analyzer
```

Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Set up environment variables:

```bash
export GEMINI_API_KEY=your_api_key_here
```

---

## Usage

Start the FastAPI server:

```bash
uvicorn main:app --reload
```

Then:

1. Upload a dataset via the API endpoint
2. Ask natural-language questions about your data
3. Receive automated insights and visualizations

Access interactive API docs at:

```
http://127.0.0.1:8000/docs
```

---

## 📊 Example Dataset & Query Format

### Example Dataset Format

The platform expects structured datasets in CSV format.  
Example (`sample-weather.csv`):

```csv
date,temperature_c,precip_mm
2024-01-01,5,0
2024-01-02,7,1
2024-01-03,6,0
2024-01-04,8,2
2024-01-05,6,0
```

---

### Example Query Format

Users submit natural-language analytical tasks along with structured output instructions.

Example query:

```
Analyze `sample-weather.csv`.

Return a JSON object with keys:
- average_temp_c: number
- max_precip_date: string
- min_temp_c: number
- temp_precip_correlation: number
- average_precip_mm: number
- temp_line_chart: base64 PNG string under 100kB
- precip_histogram: base64 PNG string under 100kB

Questions:
1. What is the average temperature in Celsius?
2. On which date was precipitation highest?
3. What is the minimum temperature recorded?
4. What is the correlation between temperature and precipitation?
5. What is the average precipitation in millimeters?
6. Plot temperature over time as a line chart with a red line. Encode as base64 PNG.
7. Plot precipitation as a histogram with orange bars. Encode as base64 PNG.
```

---

This format demonstrates how users can:

- Upload structured datasets
- Ask multi-part analytical questions
- Request statistical summaries
- Generate visualizations
- Receive structured JSON responses

## Use the Sample Dataset and Questions to try the application, which are provided in the repo
- sample-sales.csv
- sample-weather.csv
- questions-sales.txt
- questions-weather.txt

## Project Structure

```
LLM_Powered_Dataset_Analyzer/
│
├── app/
│   ├── api/
│   ├── services/
│   └── utils/
│
├── datasets/
├── main.py
├── requirements.txt
└── README.md
```

*(Update this to match your actual folder structure.)*

---

## Objectives

- Automate exploratory data analysis using LLMs
- Provide statistically grounded insights
- Enable intuitive interaction with datasets
- Improve productivity for data analysts

---

## Future Improvements

- Support for larger datasets
- Advanced visualization dashboards
- User authentication & session management
- Real-time streaming insights
- Deployment with Docker & cloud hosting

---

## 📜 License

This project is licensed under the MIT License.

---

## 👤 Author

** K Balvivek Reddy**

Feel free to connect or raise issues for suggestions and improvements!

---

## ⭐ Acknowledgements

- LangChain community
- Google Gemini API
- Open-source Python ecosystem

---

⭐ If you like this project, consider starring the repo!
