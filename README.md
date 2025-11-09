# MileageHelper

IRS-compliant mileage log enhancement tool for short-term rental property management.

## Overview

This tool automatically enhances MileIQ CSV exports with detailed, IRS-compliant business purpose descriptions. Designed specifically for short-term rental property managers operating between multiple locations.

## Features

- Analyzes trip routes and destinations to infer business purposes
- Adds detailed, audit-ready descriptions for all trips
- Context-aware logic for rental property management activities
- Generates compliance reports showing improvements
- Reusable for future MileIQ exports

## Usage

```bash
python3 enhance_mileage.py
```

The tool will:
1. Read your MileIQ CSV export
2. Analyze each trip based on start/end locations
3. Generate IRS-compliant business purpose descriptions
4. Output an enhanced CSV file with `_ENHANCED` suffix
5. Display a detailed compliance report

## Business Context

This tool is optimized for rental property management between:
- **Home Base:** State College, PA
- **Rental Properties:** Trumansburg, NY area

## Example Enhancements

| Original | Enhanced |
|----------|----------|
| *(blank)* | Travel to rental property for guest services/maintenance |
| "Business" | Multi-stop supply run for rental property maintenance |
| "Errand/Supplies" | Return to rental property with supplies and materials |

## IRS Compliance

The tool ensures all trips have:
- Specific business purpose descriptions
- References to rental property management activities
- Demonstration of business necessity
- Audit-ready documentation

## Files

- `enhance_mileage.py` - Main enhancement script
- `MileIQ__2025-08-01_2025-08-31.csv` - Sample original MileIQ export
- `MileIQ__2025-08-01_2025-08-31_ENHANCED.csv` - IRS-compliant enhanced version

## Requirements

- Python 3.x
- No external dependencies (uses standard library only)

## Tax Year 2025

Current IRS standard mileage rate: **$0.70/mile** for business use