# Eventify - Ionic React

## Description

Eventify is a mobile platform designed for event management and user interaction. It includes essential functionalities such as event administration, user connection, and social features like followers, notifications, and comments.

## Demo

[![Eventify Demo](/eventifyThumbnail.png)](https://youtu.be/5qaMUsTg-lM)

*Click on the image to watch the demo on YouTube*

## Technologies Used

- **React**: Library for building user interfaces
- **TypeScript**: Programming language that adds static typing to JavaScript
- **Capacitor**: Platform for converting web applications into native applications
- **Supabase**: Backend-as-a-service (BaaS) platform for authentication, database, and storage
- **i18next**: Internationalization solution
- **Cypress - Vitest - React Testing Library**: Libraries for unit and integration testing development

## Project Structure

```
ionic-app/
├── src/
│   ├── App.tsx                # Main application component
│   ├── assets/                # Images, fonts, and other static resources
│   ├── components/            # Reusable components
│   ├── views/                 # Main application views
│   ├── contexts/              # React Contexts
│   │   ├── AuthContext.tsx    # Authentication Context
│   │   └── PushNotificationsContext.tsx # Notifications Provider
│   ├── hooks/                 # Custom hooks
│   │   ├── useAudioRecorder.tsx # Hook for audio recording
│   │   ├── useCurrentLocation.tsx # Hook for geolocation
│   │   ├── useImagePicker.tsx # Hook for image selection
│   │   └── useFilePicker.tsx # Hook for music selection
│   ├── models/                # Interfaces and data types
│   ├── navigation/            # Navigation configuration
│   ├── i18n/                  # Internationalization configuration
│   ├── services/              # Services
│   │   ├── storage.ts         # Storage services
│   ├── styles/                # Global styles and CSS utilities
│   ├── theme/                 # Theme configuration
│   └── utils/                 # Utilities and helpers
├── public/                    # Static public files
├── capacitor.config.ts        # Capacitor configuration
├── ionic.config.json          # Ionic configuration
└── package.json               # Dependencies and scripts
```

## Prerequisites

- Node.js (v16 o higher)
- npm or yarn
- Ionic CLI
- Supabase account

## Environment Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/ruggieroDaniela/eventify-ionic.git
   cd ionic-app
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Configure environment variables:
   - Create an `.env` file in the project root
   - Add the following variables:
     ```
     VITE_SUPABASE_URL=your_supabase_url
     VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
     VITE_API_URL=your_api_url
     ```

## Running the Application

### Web Development

To start the application in web development mode:

```bash
ionic serve
```

### Device Development

To run on Android:

```bash
ionic capacitor run android -l --external
```

## Deployment

### APK Generation

To generate installation files:

```bash
ionic capacitor build android 
```

