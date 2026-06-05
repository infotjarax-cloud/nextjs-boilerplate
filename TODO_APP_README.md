# Todo App - Local Storage Task Manager

A modern, feature-rich todo list application built with Next.js, React, and Tailwind CSS. All tasks are stored locally on your device using browser localStorage.

## 🌟 Features

- ✅ **Add Tasks** - Create todos with title, description, priority, and due date
- 💾 **Local Storage** - All tasks automatically saved to your device
- ⭐ **Priority Levels** - Organize tasks by High, Medium, and Low priority
- 📅 **Due Dates** - Set due dates and track overdue tasks
- 📝 **Descriptions** - Add detailed descriptions to capture task details
- 🔄 **Filtering** - Filter tasks by All, Active, or Completed
- ✏️ **Edit Tasks** - Modify task details anytime
- 🗑️ **Delete Tasks** - Remove tasks when no longer needed
- 📊 **Statistics** - Track total, active, and completed tasks
- 🎯 **Smart Sorting** - Tasks automatically sorted by priority and completion status
- 📱 **Responsive Design** - Works perfectly on all devices
- ⚡ **Instant Updates** - All changes saved instantly

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/infotjarax-cloud/nextjs-boilerplate.git
cd nextjs-boilerplate
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

## 📁 Project Structure

```
src/
├── app/
│   ├── page.tsx              # Home/landing page
│   ├── layout.tsx            # Root layout with navigation
│   ├── globals.css           # Global styles
│   └── todo/
│       └── page.tsx          # Todo list main page
├── components/
│   ├── Navigation.tsx        # Navigation bar
│   ├── TodoForm.tsx          # Add todo form component
│   ├── TodoItem.tsx          # Individual todo item component
│   └── TodoItem.tsx          # Individual todo item component
```

## 💾 Local Storage

The app uses the browser's `localStorage` API to persist tasks. Here's how it works:

- Tasks are automatically saved to `localStorage` whenever they change
- Tasks are loaded from `localStorage` when the app starts
- No internet connection needed to access your tasks
- Data persists across browser sessions
- Clear browser cache/storage to delete all tasks

## 🎨 User Interface

### Home Page
- Landing page with feature overview
- Quick start button to todo list
- How it works section
- Call-to-action section

### Todo List Page
- Add task form with expandable options
- Task statistics (total, active, completed)
- Filter buttons (All, Active, Completed)
- Task list with sorting
- Edit and delete functionality
- Clear completed button

## 🔧 Task Properties

Each task contains:
- **id**: Unique identifier (auto-generated)
- **title**: Task name (required)
- **description**: Detailed description (optional)
- **completed**: Completion status (boolean)
- **priority**: High, Medium, or Low
- **dueDate**: Due date for the task (optional)
- **createdAt**: Task creation timestamp

## 📊 Statistics

The app displays real-time statistics:
- **Total Tasks**: All tasks in the list
- **Active Tasks**: Incomplete tasks
- **Completed Tasks**: Finished tasks

## 🎯 Filtering & Sorting

- **All**: Show all tasks
- **Active**: Show incomplete tasks
- **Completed**: Show finished tasks

Tasks are automatically sorted by:
1. Completion status (active first)
2. Priority (High → Medium → Low)

## 🛠️ Technologies Used

- **Next.js 16**: React framework
- **React 19**: UI library
- **TypeScript**: Type safety
- **Tailwind CSS 4**: Styling
- **localStorage API**: Data persistence

## 🎨 Design Features

- **Gradient backgrounds**: Modern visual design
- **Responsive layout**: Mobile, tablet, and desktop support
- **Color-coded priorities**: Visual priority indicators
- **Smooth animations**: Hover effects and transitions
- **Dark mode ready**: Can be extended for dark mode
- **Accessible**: Proper semantic HTML and ARIA labels

## 📱 Responsive Design

- Mobile-first approach
- Optimized for all screen sizes
- Touch-friendly interface
- Adaptive layouts

## 🔒 Privacy & Security

- **No server communication**: All data stays on your device
- **No account required**: Use immediately
- **No tracking**: We don't collect any data
- **No ads**: Completely ad-free
- **HTTPS ready**: Secure by default

## 🚀 Deployment

### Deploy to Vercel (Recommended)

```bash
npm install -g vercel
vercel
```

### Deploy to Other Platforms

1. **Build the app**:
```bash
npm run build
```

2. **Start the server**:
```bash
npm start
```

The app can be deployed to any platform that supports Next.js:
- Vercel
- Netlify
- AWS
- Google Cloud
- DigitalOcean
- Heroku

## 📝 Usage Examples

### Creating a Task
1. Type task title in the input field
2. Click the settings icon for more options (optional)
3. Add description, priority, and due date
4. Click "Add" button

### Editing a Task
1. Click the pencil icon (✏️) on any task
2. Update the title and description
3. Click "Save" to save changes

### Completing a Task
1. Click the checkbox next to the task
2. Task will be marked as completed
3. Task status changes in statistics

### Deleting a Task
1. Click the trash icon (🗑️) on any task
2. Task is immediately deleted

### Filtering Tasks
1. Click on "All", "Active", or "Completed" buttons
2. List updates to show filtered tasks

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests
- Improve documentation

## 📄 License

This project is open source and available under the MIT License.

## 🎉 Getting Help

- Check the [Features](#-features) section
- Review the [Usage Examples](#-usage-examples)
- Open an issue on GitHub

---

**Made with ❤️ for productivity enthusiasts**

Start organizing your tasks today! No signup, no ads, just pure productivity.
