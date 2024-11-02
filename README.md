# Video Player Simulation

## Overview

This project is a Python-based video player simulation that serves as coursework for a university project in Object-Oriented Programming (OOP). It demonstrates fundamental functionalities for a media player, including user authentication, video library management, playlist creation, and video rating. Developed using Python’s Tkinter library for the GUI, the project applies OOP principles to create a structured and user-friendly application.

## Table of Contents

- [Project Purpose and Goals](#project-purpose-and-goals)
- [Features](#features)
  - [User Authentication](#user-authentication)
  - [Video Player Interface](#video-player-interface)
  - [Playlist Management](#playlist-management)
  - [Video Metadata and Rating](#video-metadata-and-rating)
- [Design and Development](#design-and-development)
  - [Code Structure](#code-structure)
- [Testing](#testing)
- [Future Improvements](#future-improvements)
- [Installation](#installation)

---

## Project Purpose and Goals

### Purpose
This project aims to create an interactive and intuitive video player application to demonstrate OOP concepts, including inheritance, encapsulation, and polymorphism.

### Goals
The primary goal is to design a functional, Tkinter-based GUI that supports:
1. User authentication (sign-in and sign-up).
2. Video library management (view, update, and rate videos).
3. Playlist management and customization.

---

## Features

### User Authentication

The application includes:
- **Sign In/Sign Up**: Both functionalities are handled within `sign_in.py`. Users must either sign in with an existing account or sign up as a new user to access the video player.
- **User Data Storage**: Stores user credentials in an `account.csv` file and updates playlists and video ratings as the user interacts with the application.

### Video Player Interface

Upon logging in, users access the main video player screen. The GUI provides:
- **Video Browsing**: View all available videos or search by title, director, or ID.
- **Video Information Display**: Details include video ID, title, director, rating, and play count.

### Playlist Management

Users can create, modify, and reset playlists. Key functionalities include:
- **Adding Videos to Playlist**: Select videos to add to a playlist.
- **Playing Videos in Playlist**: Increments the play count for each video when played.
- **Resetting Playlist**: Clears the playlist to start afresh.

### Video Metadata and Rating

The application provides a detailed view of video information and lets users rate videos, with:
- **Star Rating System**: Allows users to rate videos from 1 to 5 stars.
- **Persistent Video Information**: Stores video data such as title, director, rating, and play count in an `account_detail.csv` file.
  
---

## Design and Development

### Code Structure

- `sign_in.py`: Manages user authentication, including both sign-in and sign-up processes. **This file must be run first for users to sign in or sign up before accessing the application.**
- `video_player.py`: Main script that initializes and runs the application, connecting all components.
- `library_item.py`: Manages the attributes of individual videos.
- `video_library.py`: Stores and manages video objects.
- `account_detail.py`: Handles user information and interactions with video data.
- `add_to_playlist.py`: Adds selected videos to the playlist.

#### Supporting Files and Folders
- **CSV Files**:
  - `account.csv`: Stores usernames and passwords.
  - `Corrected_Movie_Data.csv`: Contains video metadata.
- **Folders**:
  - `video_info`: Stores individual video descriptions.
  - `images`: Holds thumbnails for each video.

---

## Testing

This project includes a comprehensive set of tests for each feature, ensuring functionality in various scenarios. For example:
- **Sign In/Sign Up**: Tests handle correct/incorrect usernames and passwords as well as new account creation and duplicate username prevention.
- **Video Player**: Tests interaction elements like adding videos, updating ratings, and viewing playlists.

Refer to `OOP_report.pdf` for a full test table with sample inputs, actions, and expected outputs.

---

## Future Improvements

- **Video Thumbnails**: Add display of video thumbnails for better user experience.
- **Advanced Search**: Implement filters based on video metadata like year and tags.
- **Movie Recommendations**: Integrate with an API (e.g., TMDB) to suggest videos based on user ratings.
- **Admin Functions**: Add controls for admins to manage video data directly within the application.

---

## Installation

### Prerequisites
- Python 3.x
- Required libraries: Install dependencies using `pip install -r requirements.txt` (include Tkinter if necessary).

### Running the Application
1. Clone the repository.
2. Run `sign_in.py` to either sign in or sign up.
3. Once signed in, you will have access to the main application by running `video_player.py`.

---

This README provides a structured overview of the project, clarifying its purpose, design, and usage for future users or developers.
