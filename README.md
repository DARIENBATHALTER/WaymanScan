# WAA Inventory Scanner

A single-page web application for scanning and tracking WAA inventory devices.

## Features

- Upload and parse inventory CSV files
- Scan device barcodes using iPhone camera
- Manual tag entry option
- Track WAA Tags, iPad Tags, and Chromebook Tags
- Associate devices with teachers/locations
- Add condition notes for devices
- View device summary and details
- Export updated CSV with check-in information

## How to Use

1. **Setup**:
   - Open `index.html` in Safari on your iPhone
   - Upload your inventory CSV file

2. **Configure**:
   - Enter the current teacher or location name
   - Select the tag type you're scanning (WAA, iPad, or Chromebook)
   - Enable "Add condition notes" if you want to add notes for each scan

3. **Scanning**:
   - Press "Start Scanning" to activate the camera
   - Point camera at device barcode/tag
   - The app will beep and show scan results
   - For devices without readable tags, use "Enter Tag Manually"

4. **Viewing Data**:
   - Use "View All Devices" to see current inventory status
   - The summary shows check-in progress by device type

5. **Exporting**:
   - Press "Export Updated CSV" to download the current inventory data
   - The CSV will include all check-in information

## Data Persistence

The application stores all inventory data in your browser's local storage, so you can:
- Refresh the page without losing data
- Continue scanning across multiple sessions
- Upload a new CSV to replace existing data

## Requirements

- iPhone running Safari browser
- Camera access permission enabled
- CSV must have the proper format with headers:
  - Device Type
  - Make / Model
  - WAA Tag
  - iPad Tag
  - Chromebook Tag
  - Location
  - Teacher
  - Checked in? (Date and time)
  - Notes

## Troubleshooting

- If the camera doesn't start, check camera permissions in Settings
- If scanning doesn't work reliably, ensure adequate lighting and a steady hand
- For any data issues, export your current progress and restart with a fresh CSV 