# Vedic Ville: Prana Edition

A spiritual meditation and mantra chanting companion app designed to help users track their daily japa (mantra repetition) practice with a beautiful, intuitive interface.

## Features

### 🧿 Japa Tracking
- **Round Counter**: Track individual rounds of mantra chanting with an interactive mala bead counter
- **Daily Goal Setting**: Set and customize your daily round goals
- **Lifetime Statistics**: Monitor your total rounds chanted across all time
- **Cloud Logging**: All sessions are automatically saved to the cloud for persistent tracking

### 🙏 Mantra Management
- **Predefined Mantras**: Choose from popular vedic mantras including the Hare Krishna Maha-Mantra
- **Custom Mantras**: Create and save your own personalized mantras
- **Mantra Switching**: Easily switch between different mantras during your practice
- **Persistent Settings**: Your mantra preferences are saved automatically

### 🎨 Design & UX
- **Dark Mode Interface**: Eye-friendly saffron and warm gradient aesthetic
- **Breathing Circle Animation**: Visual guidance for meditation rhythm
- **Responsive Design**: Works seamlessly on mobile and desktop devices
- **Real-time Updates**: Live progress tracking with instant feedback
- **Tailwind CSS**: Modern, clean, and accessible UI styling

### 🔐 Cloud Synchronization
- **Firebase Backend**: Secure cloud storage for all user data
- **Real-time Sync**: Changes sync instantly across devices
- **Anonymous & Custom Auth**: Flexible authentication options
- **Firestore Database**: Scalable NoSQL database for user records

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Safari, Firefox, or Edge)
- Internet connection for cloud features
- Firebase configuration (required for cloud sync)

### Installation
1. Clone or download this repository
2. Open `index.html` in your web browser
3. Start tracking your japa practice immediately

### Firebase Setup (Optional)
To enable cloud synchronization and data persistence:
1. Create a Firebase project at [firebase.google.com](https://firebase.google.com)
2. Configure Firestore database and Authentication
3. Pass your Firebase configuration through the app initialization variables:
   - `__firebase_config`: Your Firebase configuration object
   - `__initial_auth_token`: Optional custom authentication token
   - `__app_id`: Application identifier

## Usage

### Tracking a Japa Session
1. Open the app in your browser
2. View your current mantra in the main display
3. Click the breathing circle or action button to increment rounds
4. Watch your daily progress update in real-time
5. Complete your session when you reach your daily goal

### Setting Your Daily Goal
1. Click on the goal settings section
2. Enter your desired number of rounds per day
3. Your goal will be saved automatically

### Choosing or Creating a Mantra
1. Access the mantra selection menu
2. Choose from predefined mantras or create a new custom mantra
3. Your selection is saved for future sessions

## Technology Stack

- **Frontend**: HTML5, CSS3 (Tailwind CSS), Vanilla JavaScript
- **Backend**: Firebase Firestore
- **Authentication**: Firebase Authentication
- **Fonts**: Google Inter Font
- **CDN**: Tailwind CSS from CDN

## Project Structure

```
index.html          # Main application file (HTML, CSS, JavaScript)
README.md          # This file
```

## Architecture

### Key Components
- **Authentication Module**: Handles Firebase authentication setup
- **Japa Listener**: Real-time listener for round logging and statistics
- **Settings Manager**: Manages goal and mantra preferences
- **Mantra System**: Handles both predefined and custom mantra management
- **UI Components**: Interactive elements for tracking and settings

### Data Structure
```
artifacts/
├── {appId}/
│   └── users/
│       └── {userId}/
│           ├── japa_logs/          # Daily japa records
│           ├── custom_mantras/     # User-created mantras
│           └── settings/
│               └── japa_settings   # Goal and current mantra
```

## Features in Detail

### Japa Logging
- Logs each completed round with timestamp
- Tracks total bead count for each session
- Automatically groups logs by date for daily statistics
- Maintains lifetime totals for long-term progress tracking

### Real-time Listeners
- Japa logs sync across all devices in real-time
- Settings changes apply instantly
- Mantra updates propagate without page refresh

### Customization
- Adjust daily round goals dynamically
- Create mantras tailored to your practice
- Customize visual aesthetics through CSS variables

## Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Android)

## Troubleshooting

### Cloud Sync Not Working
- Verify Firebase configuration is correctly passed
- Check browser console for authentication errors
- Ensure internet connection is stable

### Settings Not Saving
- Clear browser cache and reload
- Check Firebase Firestore permissions
- Verify Firebase configuration credentials

### Mantra Not Updating
- Ensure the mantra text is not empty
- Check for browser console errors
- Refresh the page if changes don't reflect

## Contributing

This is a personal spiritual practice app. For improvements or modifications, feel free to customize the code to suit your needs.

## License

Created with intention for spiritual practice and personal development.

---

**May your practice be blessed and your mantras bear fruit!** 🙏
