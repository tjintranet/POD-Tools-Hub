# POD Tools Hub

A centralized dashboard for accessing POD (Print on Demand) related tools and utilities.

## Features

- Responsive grid layout with tool cards
- Dark/Light mode toggle with persistent preferences
- Quick access to Switch and PACE systems
- Hover animations on cards
- Mobile-friendly design

## Tools Available

The hub provides access to various POD tools including:
- Item Template Creator
- Order Processing Tool
- Volume Set Manager
- Ulverscroft Item Templates
- POD Availability Checker
- TF Metadata Editor
- DHL Order CSV Creator
- Batch Size Validator
- History Press Order Viewer
- Hachette Tools
- XML Parser
- Product Spec Validator
- Book Weight Calculator
- Spine Size Calculator
- PACE Metadata to XML for DBS
- Cased POD Order Filter

## Technical Details

### Dependencies
- Bootstrap 5.3.2
- Bootstrap Icons 1.11.3
- Google Fonts (Roboto)

### Local Storage
- Theme preference is saved using localStorage
- Key: 'theme'
- Values: 'light' or 'dark'

### Browser Support
- Modern browsers supporting ES6
- Flexbox and CSS Grid
- CSS Custom Properties

## Installation

1. Clone the repository
2. Open index.html in a web browser
3. No build process required

## Development

To add new tools:
1. Copy an existing card template from index.html
2. Update icon, title, description, and link
3. Place within the grid container