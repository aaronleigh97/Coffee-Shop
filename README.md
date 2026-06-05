# Coffee Shop Review App

A React Native mobile application developed for a university project.  
The app allows users to register, log in, browse coffee shop locations, view reviews, favourite locations, like reviews, add their own reviews, and manage their user profile.

## Project Overview

This project is a mobile coffee shop review application built with React Native. It connects to a REST API backend and demonstrates core mobile development concepts such as screen navigation, authentication, persistent token storage, API requests, list rendering, and user interaction.

The application is designed around a simple user journey:

1. A user creates an account or logs in.
2. The authentication token and user ID are stored locally.
3. The user can browse coffee shop locations.
4. The user can view details and reviews for each location.
5. The user can favourite locations and like reviews.
6. The user can add their own review.
7. The user can edit their profile details.
8. The user can log out.

## Features

### Authentication

- Register a new user account
- Log in with email and password
- Store authentication token locally using AsyncStorage
- Store user ID locally using AsyncStorage
- Log out and clear local storage

### Location Browsing

- Fetch coffee shop locations from the backend API
- Display locations in a scrollable list
- Sort locations alphabetically
- Show basic location information, including town and average rating
- Navigate from a location to its detailed review screen

### Favourites

- View a list of favourite coffee shop locations
- Display favourite status using heart icons
- Favourite or unfavourite a location from the review screen

### Reviews

- View reviews for a selected coffee shop location
- View location rating information, including overall, price, quality, and cleanliness ratings
- Like or unlike individual reviews
- Display review like counts
- Add a new review for a location

### Add Review

Users can submit a review containing:

- Overall rating
- Price rating
- Quality rating
- Cleanliness rating
- Written review body

### Profile Management

- Fetch the logged-in user's profile details
- Edit first name, last name, email, and password
- Submit profile updates to the backend API

## Technologies Used

- React Native
- JavaScript
- React Navigation
- React Native Elements
- AsyncStorage
- Jest
- React Test Renderer
- ESLint
- Standard style guide

## Main Dependencies

The project uses:

- `react`
- `react-native`
- `@react-navigation/native`
- `@react-navigation/stack`
- `@react-navigation/drawer`
- `@react-native-async-storage/async-storage`
- `react-native-elements`
- `react-native-vector-icons`
- `react-native-gesture-handler`
- `react-native-reanimated`
- `react-native-screens`
- `jest`
- `react-test-renderer`

## Project Structure

```text
Project/
│
├── App.js
├── index.js
├── app.json
├── package.json
├── README.md
│
├── components/
│   ├── addReview.js
│   ├── favourites.js
│   ├── home.js
│   ├── locations.js
│   ├── login.js
│   ├── profile.js
│   ├── register.js
│   └── reviews.js
│
├── __tests__/
│   └── App-test.js
│
├── android/
└── ios/
