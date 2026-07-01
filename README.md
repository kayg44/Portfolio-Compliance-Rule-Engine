# Portfolio Compliance Rule Engine

A Python and SQL-based portfolio compliance monitoring tool that automates investment guideline validation across portfolio holdings.

---

## Overview

Portfolio compliance is a critical function in asset management, ensuring investment portfolios remain within client mandates and regulatory constraints. As portfolios grow in size and complexity, manually reviewing every holding becomes increasingly time-consuming and susceptible to human error.

This project demonstrates how portfolio compliance can be automated by translating investment guidelines into executable Python and SQL logic. The rule engine evaluates portfolio holdings against predefined investment restrictions, identifies breaches, and generates a structured compliance report for review.

Although simplified, the workflow reflects the core principles used by institutional asset managers to automate compliance monitoring.

---

## Why I Built This

I built this project to better understand how investment firms automate portfolio compliance and investment guideline monitoring.

Rather than simply analyzing portfolio performance, I wanted to explore how technology can be used to convert written investment mandates into repeatable business rules. This project combines finance, data analysis, Python, and SQL to simulate a simplified compliance workflow commonly used in institutional asset management.

---

## Business Value

Traditional compliance reviews often require analysts to manually inspect portfolio holdings against numerous investment guidelines. As the number of holdings increases, this process becomes slower, less scalable, and more prone to oversight.

This rule engine demonstrates how automation can improve that process by:

- Automating repetitive compliance checks
- Identifying portfolio breaches within seconds
- Applying investment rules consistently across all holdings
- Reducing manual review effort
- Producing structured compliance reports for decision-making
- Improving transparency through clearly documented rule violations

The project illustrates how technology can improve operational efficiency while supporting faster and more consistent compliance monitoring.

---

## Technologies Used

- Python
- Pandas
- SQLite
- SQL
- Google Colab

---

## Portfolio Data

The project uses a mock investment portfolio consisting of equities, bonds, and cash.

Each holding contains:

- Ticker
- Security Name
- Asset Class
- Sector
- Credit Rating
- Portfolio Weight (%)
- Market Value

---

## Investment Rules Tested

The current rule engine evaluates three investment guidelines.

### Position Concentration

No individual security may exceed **5%** of the total portfolio.

---

### Sector Concentration

Technology sector exposure is monitored to ensure it remains below the defined concentration threshold.

---

### Credit Quality

Bond holdings must maintain a minimum investment-grade credit rating of **BBB-** or higher.

---

## How It Works

1. A mock investment portfolio is created using Pandas.
2. Python evaluates each holding against predefined investment rules.
3. Portfolio data is stored in a SQLite database.
4. SQL queries perform the same compliance checks directly against the database.
5. Results from both Python and SQL are consolidated into a single compliance report.
6. Holdings are labelled as compliant or violating based on the applicable investment guidelines.
7. A final compliance report is exported for review.

---

## Example Output

The compliance report includes:

- Compliance rule evaluated
- Portfolio holding
- Asset class
- Sector
- Credit rating
- Portfolio weight
- Market value
- Violation description
- Compliance source (Python or SQL)

Holdings that violate investment guidelines are automatically highlighted, allowing portfolio managers and compliance professionals to quickly identify and investigate potential breaches.

---

## Skills Demonstrated

- Portfolio Compliance
- Investment Guideline Monitoring
- Python Programming
- SQL Querying
- Data Analysis
- Business Rule Automation
- Financial Data Processing
- SQLite
- Pandas

---

## What I Learned

This project gave me a deeper understanding of how portfolio compliance operates within institutional asset management.

I learned how written investment guidelines can be translated into automated business logic using Python and SQL, allowing portfolios to be monitored consistently and efficiently. The project also reinforced the complementary strengths of Python for implementing business logic and SQL for querying structured portfolio data.

Most importantly, I gained a greater appreciation for how automation can reduce manual effort, improve consistency, and support more efficient investment operations.

---

## Future Improvements

Potential enhancements include:

- Configurable investment guidelines loaded from external files
- Additional issuer, country, and ESG concentration rules
- Interactive dashboard using Streamlit
- Automated PDF compliance reporting
- Live market data integration
- Support for larger institutional portfolios

---

## Running the Project

Clone the repository:

```bash
git clone https://github.com/kayg44/portfolio-compliance-rule-engine.git
```

Install dependencies:

```bash
pip install pandas
```

Open the notebook in Google Colab or Jupyter Notebook and run all cells.

The notebook will automatically:

- Create the mock portfolio
- Execute compliance checks
- Generate the compliance report

---

## Author

**Kwasi Asante**

Data Analytics | Finance | Python | SQL
