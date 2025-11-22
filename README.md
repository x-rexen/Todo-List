# Advanced Todo List - README

## 📋 Overview

A feature-rich, responsive todo list application with advanced task management capabilities. Organize your tasks with custom types, dates, and time periods in a clean, modern interface.

## ✨ Features

### 🎯 Task Management
- **Add Tasks** with titles, descriptions, dates, and times
- **Set Time Periods** for tasks with start and end dates
- **Mark Tasks** as complete/incomplete with visual indicators
- **Delete Tasks** individually or clear all completed tasks
- **Filter Tasks** by type and completion status

### 🏷️ Custom Task Types
- **Create Custom Types** with unique names and colors
- **Visual Type Indicators** with color-coded badges
- **Manage Types** - add new types or delete existing ones
- **Type-based Filtering** to view tasks by category

### 📅 Multiple View Options
- **List View**: Traditional task listing with sorting options
- **Date View**: Tasks grouped by date with chronological organization
- **Type View**: Tasks grouped by custom types with color coding

### 💾 Data Persistence
- **Local Storage**: All data automatically saved in browser
- **No Fake Data**: Clean start with only default task types
- **Persistent State**: Tasks and types remain between sessions

### 🎨 User Experience
- **Responsive Design** works on desktop and mobile devices
- **Smooth Animations** and transitions for better interaction
- **Visual Feedback** with notifications for all actions
- **Statistics Dashboard** showing task completion metrics
- **Intuitive Interface** with clear visual hierarchy

## 🚀 Getting Started

### Prerequisites
- Modern web browser with JavaScript enabled
- No additional installations required

### Installation
1. Download the `index.html` file
2. Open it in your web browser
3. Start organizing your tasks immediately!

## 📖 How to Use

### Adding Tasks
1. Fill in the task title (required)
2. Add an optional description
3. Select a task type from the dropdown
4. Set a date and/or time (optional)
5. Enable "Set Time Period" for tasks spanning multiple days
6. Click "Add Task" to save

### Managing Task Types
1. Enter a type name in the "Type Name" field
2. Choose a color using the color picker
3. Click "Add Type" to create
4. Use the delete button next to any type to remove it

### Filtering and Views
- Use the **Type Filter** to show tasks by specific categories
- Use the **Status Filter** to show All, Pending, or Completed tasks
- Switch between **List, Date, and Type Views** using the view options
- **List View**: All tasks in a single scrollable list
- **Date View**: Tasks grouped by their due dates
- **Type View**: Tasks organized by custom categories

### Task Actions
- **Complete/Incomplete**: Click the checkbox or "Mark Complete" button
- **Delete**: Use the delete button on individual tasks
- **Clear Completed**: Remove all completed tasks at once

## 🛠️ Technical Details

### Built With
- **HTML5** - Structure and semantics
- **CSS3** - Styling with CSS Grid and Flexbox
- **Vanilla JavaScript** - Functionality and data management
- **Font Awesome** - Icons for better UX
- **Local Storage API** - Data persistence

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Data Structure
```javascript
// Task Types
{
  id: number,
  name: string,
  color: string (hex code)
}

// Tasks
{
  id: number,
  title: string,
  description: string,
  typeId: number,
  date: string (YYYY-MM-DD),
  time: string (HH:MM),
  period: {
    startDate: string,
    endDate: string
  },
  completed: boolean,
  createdAt: string (ISO date)
}
```

## 🔧 Customization

### Adding Default Task Types
Modify the `loadData()` function to include your preferred default types:

```javascript
taskTypes = [
  { id: 1, name: 'Work', color: '#4361ee' },
  { id: 2, name: 'Personal', color: '#4cc9f0' },
  { id: 3, name: 'Shopping', color: '#f72585' },
  // Add more types as needed
];
```

### Styling Customization
The application uses CSS custom properties for easy theming. Modify the `:root` variables in the CSS to change colors, spacing, and other design elements.

## 📱 Mobile Support

The application is fully responsive and includes:
- Touch-friendly interface elements
- Optimized layouts for mobile screens
- Accessible design patterns
- Smooth scrolling and interactions

## 🔒 Data Privacy

- All data is stored locally in your browser
- No data is sent to external servers
- Complete control over your information
- Easy data reset by clearing browser storage

## 🐛 Troubleshooting

### Common Issues
1. **Tasks not saving**: Ensure JavaScript is enabled
2. **Filter not working**: Check that tasks have the selected type assigned
3. **Views not updating**: Refresh the page to reset the application state

### Resetting Data
To completely reset the application:
1. Open browser Developer Tools (F12)
2. Go to Application tab → Storage → Local Storage
3. Right-click and "Clear" the domain storage
4. Refresh the page

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📞 Support

If you encounter any problems or have questions:
1. Check the troubleshooting section above
2. Ensure you're using a supported browser
3. Try resetting the application data

---

**Enjoy staying organized with your new Advanced Todo List!** 🎉
