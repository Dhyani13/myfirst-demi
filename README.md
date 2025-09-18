# Sports App

A Flutter application for tracking sports activities and workouts with pose detection capabilities.

## Overview

This application allows users to track their workouts, upload selfies, and analyze their performance using pose detection. It connects to a backend API for data storage and authentication.

## Configuration

The application uses a `config.json` file in the root directory for configuration. Currently, it supports the following parameters:

```json
{
  "API_URL": "https://api.example.com"
}
```

### API Configuration

The `API_URL` parameter specifies the base URL for the backend API. This is used throughout the application for all API calls.

### API Endpoints

The application uses the following API endpoints:

- Authentication:
  - `POST /api/v1/auth/register` - Register a new user
  - `POST /api/v1/auth/login` - Login an existing user

- User Profile:
  - `GET /api/v1/profile` - Get user profile
  - `PUT /api/v1/profile` - Update user profile

- Workouts:
  - `POST /api/v1/workouts` - Create a new workout
  - `GET /api/v1/workouts` - Get user workouts

- Statistics:
  - `GET /api/v1/stats` - Get user statistics

- Selfies:
  - `POST /api/v1/selfie/upload` - Upload a selfie
  - `DELETE /api/v1/selfie` - Delete a selfie

## Project Structure

- `lib/core/`: Core functionality including API services, configuration, and user management
- `lib/features/`: Feature-specific code including pose detection
- `lib/ui/`: User interface components and screens
- `lib/widgets/`: Reusable widgets used throughout the app

## Getting Started

1. Ensure you have Flutter installed on your machine
2. Clone this repository
3. Update the `config.json` file with your API URL
4. Run `flutter pub get` to install dependencies
5. Run `flutter run` to start the application

## Troubleshooting

For common issues and their solutions, please refer to the `TROUBLESHOOTING.md` file in the root directory.

## Development

This project uses Firebase for authentication and storage. Make sure to configure Firebase properly for your environment.

For more detailed information about the implementation, see `DART_IMPLEMENTATION_SUMMARY.md`.
