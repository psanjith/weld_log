# Weld & NDE Log - Interactive Form Web App

A modern web application for data entry with Excel integration. Upload your Excel template, fill in the form fields, and export your data back to Excel.

## Features

✨ **Key Features:**
- 📤 Upload Excel files with headers (yellow row)
- 📝 Interactive form with dynamic fields from Excel headers
- 📊 Real-time data grid display
- ✏️ Edit and delete rows
- ⬇️ Export data back to Excel
- 📱 Responsive design (works on desktop and mobile)
- 💾 In-memory data storage (persists during session)

## Quick Start

### Method 1: Using Python (Recommended)

```bash
cd /Users/prakul/Downloads/projects/ai-desktop-companion/backend/weldlog_appa
python3 server.py
```

Then open your browser to: `http://localhost:8000`

### Method 2: Using Node.js

```bash
cd /Users/prakul/Downloads/projects/ai-desktop-companion/backend/weldlog_appa
npx http-server
```

### Method 3: Direct File Access

Simply open `index.html` in your web browser (some features may be limited due to browser security)

## How to Use

1. **Prepare Your Excel File:**
   - Create an Excel sheet with headers in the first row
   - Format the header row with yellow background (optional but recommended)
   - The app will read these headers as form fields

2. **Upload:**
   - Click "📁 Upload Excel File" button
   - Select your Excel file (.xlsx or .xls)
   - The form will auto-populate with fields based on headers

3. **Enter Data:**
   - Fill in the form fields with your data
   - Click "✅ Add Row" to add the entry to the grid

4. **Manage Data:**
   - View all entries in the data grid
   - Click "Edit" to modify an existing row
   - Click "Delete" to remove a row

5. **Export:**
   - Click "⬇️ Export to Excel" to download your data
   - The exported file will have the same structure with headers in yellow

## File Structure

```
weldlog_appa/
├── index.html      # Main web application (HTML, CSS, JavaScript)
├── server.py       # Python HTTP server
└── README.md       # This file
```

## Technical Details

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Excel Handling:** XLSX.js library (client-side)
- **Server:** Python built-in HTTP server (optional, for better CORS handling)
- **Browser Support:** All modern browsers (Chrome, Firefox, Safari, Edge)

## Requirements

- Modern web browser (for the app itself)
- Python 3.x (if using the Python server)
- Excel file with headers in the first row

## Tips

- **Backup Your Data:** Always export your data regularly to avoid losing entries
- **Template Format:** Keep your Excel template simple with text data
- **Performance:** The app works best with up to 1000 rows of data
- **Offline Usage:** The app works completely offline once loaded

## Troubleshooting

**File upload not working:**
- Make sure you're using a modern browser
- Check that the Excel file is not corrupted
- Try a different Excel file to test

**Export not working:**
- Ensure you have at least one data entry
- Check browser console for errors (F12)
- Try a different browser

**Form fields not appearing:**
- Verify the Excel file has headers in the first row
- Make sure the headers are not empty
- Check browser console for any error messages

## Support

For issues or questions, check that:
1. You're using a supported browser (Chrome, Firefox, Safari, or Edge)
2. The Excel file is in .xlsx or .xls format
3. The headers row is the first row in the Excel sheet

Enjoy using the Weld & NDE Log Form! 🎉
