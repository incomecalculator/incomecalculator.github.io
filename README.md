# 💰 Income Calculator

A web-based deposit income calculator designed for Ukrainian bank deposits. Calculate and compare your potential earnings with automatic tax deductions.

🔗 **Live Demo:** [https://incomecalculator.github.io](https://incomecalculator.github.io)

## 📋 Description

Income Calculator helps users in Ukraine calculate potential income from bank deposits. It supports multiple currencies, accounts for the 23% tax rate on deposit income, and allows side-by-side comparison of different deposit scenarios.

## ✨ Features

- **Multi-Currency Support**
  - UAH (Ukrainian Hryvnia) - 3% to 19% annual rates
  - USD (US Dollar) - 0.1% to 3% annual rates
  - EUR (Euro) - 0.1% to 3% annual rates

- **Flexible Calculations**
  - Initial deposit amount
  - Monthly contributions
  - Customizable period (1-60 months)
  - Adjustable interest rates

- **Automatic Tax Calculation**
  - 23% tax rate on deposit income (Ukrainian tax law)
  - Shows gross income, tax amount, and net income

- **Comparison Tool**
  - Compare up to 3 different deposit scenarios
  - Identifies the best option based on return percentage
  - Side-by-side results display

- **History Tracking**
  - Saves calculation history (last 12 entries)
  - Saves comparison history
  - Persistent storage using localStorage

- **Modern UI/UX**
  - Dark theme design
  - Responsive layout (mobile, tablet, desktop)
  - Smooth animations
  - Custom modal dialogs

## 🚀 Usage

1. Select your currency (UAH, USD, or EUR)
2. Enter the initial deposit amount
3. Optionally add monthly contributions
4. Set the deposit period in months
5. Adjust the annual interest rate using the slider
6. Click "Calculate Income" to see results

### Comparing Deposits

1. Calculate at least 2 different deposits
2. Ensure the "Compare" checkbox is selected for each
3. Click "Compare Selected Calculations"
4. View side-by-side comparison with the best option highlighted

## 🛠️ Installation

No installation required. Simply open `index.html` in a web browser.

For local development:

```bash
git clone https://github.com/incomecalculator/incomecalculator.github.io.git
cd incomecalculator.github.io
```

Then open `index.html` in your browser.

## 📁 Project Structure

```
incomecalculator.github.io/
├── index.html      # Main application file (HTML, CSS, JS)
└── README.md       # Documentation
```

## 🧮 Calculation Formula

The calculator uses compound interest with monthly contributions:

```
For each month:
  Monthly Interest = Current Balance × (Annual Rate / 12)
  New Balance = Current Balance + Monthly Interest + Monthly Contribution

Tax = Total Interest × 0.23
Net Income = Total Interest - Tax
Final Amount = Total Deposited + Net Income
```

## 🌐 Localization

- Interface: English
- Target market: Ukraine
- Tax rate: 23% (Ukrainian deposit income tax)

## 📱 Responsive Design

- **Mobile:** Single calculator view, 2 calculators for comparison
- **Tablet:** 2 calculators side by side
- **Desktop:** 3 calculators with full comparison features

## 💾 Data Storage

All data is stored locally in the browser using `localStorage`:
- Calculator settings and results
- Calculation history (max 12 entries)
- Comparison history (max 12 entries)

No data is sent to external servers.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

MIT License

## 🔗 Links

- **Repository:** [https://github.com/incomecalculator/incomecalculator.github.io](https://github.com/incomecalculator/incomecalculator.github.io)
- **Live Application:** [https://incomecalculator.github.io](https://incomecalculator.github.io)

## ⚠️ Disclaimer

This calculator is provided for informational purposes only. Actual deposit rates and terms may vary between banks. Tax regulations may change. Please consult with your bank and tax advisor for accurate financial planning.
