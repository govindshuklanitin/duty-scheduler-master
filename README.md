# Duty Scheduler

A modern web application to easily generate and manage shift schedules for employees.

![Duty Scheduler](https://i.imgur.com/JxEiFvf.png)

## Features

- **Interactive UI**: Beautiful, responsive design that works on desktop and mobile devices
- **Simple Schedule Generation**: Easily create duty schedules with automatic shift rotation
- **Multiple Shifts Support**: Handles various shift types (Morning, Afternoon, Night, General)
- **Rest Day Management**: Configure different rest days for each employee
- **Excel Export**: Export schedules to professionally formatted Excel spreadsheets
- **Performance Optimized**: Fast schedule generation with caching for repeated requests
- **User-Friendly Alerts**: Provides helpful feedback through notifications
- **Visual Schedule**: Color-coded shifts for easy readability
- **Error Handling**: Robust error handling throughout the application

## Technology Stack

- **Backend**: Flask 2.2.3 (Python web framework)
- **Frontend**: HTML5, CSS3, JavaScript with Bootstrap 5
- **Styling**: Custom CSS with modern design patterns
- **Spreadsheet Generation**: OpenPyXL 3.1.2
- **Deployment Ready**: Configured for Heroku and other platforms

## Setup and Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/duty-scheduler.git
   cd duty-scheduler
   ```

2. Create a virtual environment (recommended):
   ```
   python -m venv venv
   ```

3. Activate the virtual environment:
   - On Windows:
     ```
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```
     source venv/bin/activate
     ```

4. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

5. Run the application:
   ```
   python app.py
   ```

6. Open your web browser and navigate to:
   ```
   http://localhost:5000
   ```

## Usage Guide

1. **Select Month and Year**: Choose the month and year for the schedule
2. **Add Employees**: Fill in employee details including:
   - Name
   - Code number
   - Post (Supervisor or Helper)
   - Starting shift (A, B, C, or G)
   - Rest day (day of the week)
3. **Generate Schedule**: Click "Generate Schedule" to create the duty roster
4. **Review Schedule**: View the color-coded schedule in the browser
5. **Export to Excel**: Click "Export to Excel" to download a formatted spreadsheet

## Environment Variables

You can configure the application using the following environment variables:

- `PORT`: Port number to run the application (default: 5000)
- `FLASK_DEBUG`: Set to 'true' to enable debug mode
- `ENABLE_PROFILING`: Set to '1' to enable performance profiling

## Performance Optimization

The application includes several performance optimizations:

- **LRU Caching**: Caches schedule generation results for repeated requests
- **Pre-calculation**: Pre-calculates weekdays to reduce computation in loops
- **Efficient DOM Manipulation**: Uses modern JavaScript for efficient UI updates
- **Loading Indicators**: Provides visual feedback during processing

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to everyone who has contributed to making this project better
- Icons provided by Font Awesome
- UI components from Bootstrap
