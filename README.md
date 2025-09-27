# POD Tools Hub

A centralized dashboard for accessing POD (Print on Demand) related tools and utilities with an enhanced user experience featuring favorites management and smooth animations.

## Features

- **Responsive grid layout** with animated tool cards
- **Dark/Light mode toggle** with persistent preferences
- **Favorites system** - Bookmark frequently used tools and filter view
- **Enhanced card animations** - Cards pop out with shadow effects on hover
- **Quick access** to Switch and PACE systems
- **Mobile-friendly design**
- **Persistent user preferences** across browser sessions

## User Interface Enhancements

### Card Animations
- Cards lift up and scale slightly when hovered
- Dynamic shadow effects for depth perception
- Smooth 0.3s transitions for all animations

### Favorites System
- Click the bookmark icon on any card to mark as favorite
- Bookmarks turn red when active
- Use the filter toggle in the header to switch between "All" and "Favorites" view
- All preferences saved automatically in localStorage

### Theme Toggle
- Sun/moon icon in header for quick theme switching
- Gradient backgrounds in dark mode
- Consistent sizing and visual feedback

## Tools Available

The hub provides access to various POD tools including:

### Template & Item Creation
- Item Template Creator
- Ulverscroft Item Templates

### Order Processing
- Manual Order Processing
- Clays Daily POD Orders
- Clays Daily ASR Orders
- History Press Order Viewer

### Volume & Set Management
- Volume Set Creator
- Volume Set Search
- Vol Set Reverse Search

### Metadata & Validation
- TF Metadata Editor
- T&F Batch Validator
- T&F Product Validation

### Hachette Tools
- Hachette Inbound Order Checker
- Hachette Order Response Checker
- Make Hachette .PBS File
- Make Hachette .PPR File
- Split Hachette Order Files

### Clays Tools
- Clays 1up to Titan
- Clays POD CS WTL
- Clays Specification Code Decoder
- Clays ASR Book Spec Search

### Utilities
- POD Availability Checker

## Technical Details

### Dependencies
- Bootstrap 5.3.2
- Bootstrap Icons 1.11.3
- Google Fonts (Roboto)

### Local Storage
The application uses localStorage to persist user preferences:
- **Theme preference**: `'theme'` - Values: `'light'` or `'dark'`
- **Favorites list**: `'podToolsFavorites'` - Array of tool IDs
- **Filter state**: `'showOnlyFavorites'` - Boolean: `'true'` or `'false'`

### Browser Support
- Modern browsers supporting ES6
- Flexbox and CSS Grid
- CSS Custom Properties
- localStorage API

### Styling Features
- CSS transitions and transforms
- Gradient backgrounds
- Dynamic box shadows
- Bootstrap utility classes
- Custom CSS for enhanced UX

## Installation

1. Clone the repository
2. Open index.html in a web browser
3. No build process required - runs directly in browser

## Development

### Adding New Tools
1. Copy an existing card template from index.html
2. Update the following attributes:
   - `data-tool-id`: Unique identifier for the tool
   - Icon class (Bootstrap Icons)
   - Card title
   - Card description
   - Tool URL
3. Place within the `.row.g-3` grid container

### Card Template
```html
<div class="col-md-4 col-lg-3">
    <div class="card tool-card" data-tool-id="unique-tool-id">
        <i class="bi bi-bookmark-fill favorite-star" onclick="toggleFavorite(event, 'unique-tool-id')"></i>
        <div class="card-body text-center">
            <i class="bi bi-icon-name card-icon"></i>
            <h5 class="card-title">Tool Name</h5>
            <p class="card-text">Tool Description</p>
            <a href="tool-url" class="btn btn-primary btn-sm">Open</a>
        </div>
    </div>
</div>
```

### Customizing Styles
Key CSS classes for customization:
- `.tool-card` - Main card styling and hover effects
- `.favorite-star` - Bookmark icon styling
- `.filter-toggle` - Filter button styling
- `.theme-toggle` - Theme switcher styling

## Usage

1. **Browse Tools**: Scroll through the grid to see all available tools
2. **Bookmark Favorites**: Click the bookmark icon on cards you use frequently
3. **Filter View**: Click the filter button (with funnel icon) to toggle between all tools and favorites
4. **Switch Themes**: Click the sun/moon icon to toggle between light and dark modes
5. **Open Tools**: Click the "Open" button on any card to launch the tool

## Future Enhancements

Potential features for future development:
- Search functionality
- Tool categories/tags
- Usage statistics
- Tool descriptions and help tooltips
- Keyboard shortcuts
- Export/import favorites
- User profiles