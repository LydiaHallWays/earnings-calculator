# 📊 Earnings Calculator

A **client-side web application** for calculating net earnings from CSV files. All processing happens in your browser - no data is sent to any servers!

## 🌟 Features

- **100% Client-Side**: All calculations done in your browser using JavaScript
- **No Backend Required**: Works as a static website - perfect for GitHub Pages
- **Privacy First**: Your CSV data never leaves your device
- **Configurable Chatter's Cut**: Set any percentage (0-100%) with real-time updates
- **UK Timezone Support**: Automatically converts UTC timestamps to UK time (GMT/BST)
- **Date Range Filtering**: Filter transactions by UK date ranges
- **Referral Separation**: Separate tracking for referral vs. regular income
- **Beautiful UI**: Responsive design with drag-and-drop file upload
- **Error Handling**: Comprehensive validation and helpful error messages
- **Zero Dependencies**: Pure vanilla JavaScript with built-in CSV parsing

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended)

1. **Fork this repository**
2. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Select "Deploy from a branch" → `main` → `/ (root)`
3. **Visit your site**: `https://yourusername.github.io/earnings-calculator`

### Option 2: Local Development

```bash
# Clone the repository
git clone https://github.com/yourusername/earnings-calculator.git
cd earnings-calculator

# Serve locally (any web server works)
python3 -m http.server 8000
# OR
npx serve .
# OR just open index.html in your browser
```

## 📁 Project Structure

```
earnings-calculator/
├── index.html              # Complete web application
└── README.md               # This file
```

## 📊 CSV Format

Your CSV file must contain a **"Net"** column with numeric values. Optional columns for enhanced features:

```csv
Net,Tax,Fanvue Fee,Price,Gross,Invoice Number,Paid At (UTC),Type,Fan Handle
3.24,0,0.81,4.05,4.05,FVE-20250916-17028,2025-09-16 12:45:27,Subscription,user1
16.79,0,4.2,20.99,20.99,FVE-20250916-2525,2025-09-16 01:47:05,Message,user2
40.00,0,10,50,50,FVE-20250915-37892,2025-09-15 23:23:51,Tip,user3
5.50,0,1.5,7.00,7.00,FVE-20250916-12345,2025-09-16 14:30:00,Referral,user4
```

### Column Details:
- **Net** (Required): Numeric values for earnings calculation
- **Paid At (UTC)** (Optional): UTC timestamps automatically converted to UK time (GMT/BST)
- **Type** (Optional): Transaction type - "Referral" transactions are calculated separately

## ✨ How It Works

1. **Upload**: Drag and drop or click to select your CSV file
2. **Filter** (Optional): Set date range to filter transactions by UK dates
3. **Parse**: JavaScript reads and parses the CSV entirely in your browser
4. **Configure** (Optional): Set your custom "chatter's cut" percentage (defaults to 35%)
5. **Calculate**: Processes transactions with these features:
   - Converts UTC timestamps to UK timezone (GMT/BST)
   - Separates referral transactions from regular earnings
   - Calculates your configurable percentage of net earnings
6. **Display**: Shows three key metrics with real-time percentage updates

## 🔒 Privacy & Security

- **No Server Required**: All processing happens client-side
- **No Data Upload**: Your CSV file never leaves your device
- **No External Dependencies**: No third-party libraries or CDNs
- **Works Offline**: Save the HTML file and use it anywhere

## 🌐 Live Demo

**[Try it now!](https://yourusername.github.io/earnings-calculator)** (replace with your GitHub Pages URL)

## 🎯 Use Cases

- **Freelancers**: Calculate total earnings from client invoices
- **Content Creators**: Sum up platform earnings
- **Small Businesses**: Quick revenue calculations
- **Personal Finance**: Track income from various sources

## 🔧 Technical Details

- **Pure JavaScript**: No frameworks or libraries
- **Built-in CSV Parser**: Handles quoted fields and edge cases
- **Error Handling**: Validates CSV format and data types
- **Responsive Design**: Works on desktop and mobile
- **Modern Browser Features**: Uses File API and async/await

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test with your own CSV files
5. Submit a pull request

## 📋 FAQ

**Q: Do you store my CSV data?**
A: No! All processing happens in your browser. No data is sent anywhere.

**Q: What browsers are supported?**
A: Modern browsers that support the File API (Chrome, Firefox, Safari, Edge).

**Q: Can I use this offline?**
A: Yes! Save the `index.html` file and open it in any browser.

**Q: What if my CSV has a different structure?**
A: The calculator looks for a column named "Net". Make sure your CSV has this column header.

## 📄 License

MIT License - feel free to use this project for any purpose.

---

**No servers, no complexity, just simple CSV calculations in your browser!** 🎉
