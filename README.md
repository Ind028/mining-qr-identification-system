# Mining QR Identification System

## What is this?

This system helps mining operations track vehicles and equipment using QR codes that can withstand harsh mining conditions (dust, vibration, low light, motion blur). It generates QR codes with realistic mining data, tests them under 11 different environmental conditions, and provides a real-time scanner that logs scans to Excel.

## How It Works

1. **Generate QR Codes** - Creates 15 unique QR codes with random mine IDs, equipment types, and fleet numbers (e.g., `MINE01|DUMPTRUCK123|FLEET-A`)

2. **Test Conditions** - Automatically tests QR readability under:
   - Dust (15% & 25%)
   - Motion blur (10km/h & 20km/h)
   - Low light / Sun glare
   - Vibration / Mud / Rain / Scratches

3. **Scan QR Codes** - Live camera scanner with adjustable speed, stability detection, and automatic Excel logging

## Quick Start

### 1. Install Requirements
```bash
pip install qrcode[pil] opencv-python numpy matplotlib openpyxl
