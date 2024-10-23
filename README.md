
![Header](https://capsule-render.vercel.app/api?type=venom&height=300&color=gradient&text=Holly%20Quran%20App&fontColor=0c0)

The Holly Quran App is a mobile application built using Flutter that allows users to easily read and search the Holy Quran. This app provides several useful features including searching for surahs (سور) by name or number, searching by parts (الأجزاء), and adding bookmarks for easy reference.



## Features

- **Surah List**: Displays a list of Surahs from the Quran with their English names.
- **Search Functionality**: Users can search Surahs by typing in the search bar, and the results are filtered dynamically.
- **Dark Mode Support**: The app adjusts its appearance based on the current theme (light or dark).
- **Error Handling and Retry**: If there's an error in fetching Surah data, the app shows a retry button to fetch the data again.
- **Animations**: Flare animations are used to enhance the UI in dark mode.

## Technologies Used

- **Flutter**: For building the mobile UI.
- **Bloc (flutter_bloc)**: To manage the state of the application using `ChapterCubit`.
- **Provider**: For handling theme changes (dark mode/light mode).
- **Animations**: Flare is used to add animated effects in dark mode.
- **Iconsax**: For modern iconography within the UI.
- **Material Design**: Follows Material Design principles for consistent UI/UX.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/al-quran-surah-index.git

   
2. **Navigate to the project directory**:

   ```bash
   cd al-quran-surah-index
   
3. **Install dependencies**:
Ensure you have Flutter installed and run:

   ```bash
   flutter pub get
   
4. **Run the app**:
Use the following command to run the app on your preferred device or emulator:

   ```bash
   flutter run

## Project Structure

The project is structured as follows:

```plaintext
lib/
├── configs/              # Configuration files for the app.
├── cubits/               # State management cubits (e.g., ChapterCubit).
├── models/               # Data models (Chapter, Juz, etc.).
├── providers/            # Providers (e.g., AppProvider for theme management).
├── ui/
│   ├── animations/       # Custom animations for the app.
│   ├── widgets/          # Reusable UI widgets (buttons, titles, etc.).
│   └── surah_index/      # Main Surah Index screen and its components.
└── utils/                # Utility files (assets, helper methods, etc.).


## Key Files

- **`surah_index_screen.dart`**: This file contains the main UI logic for displaying the Surah index and handling search functionality.
- **`chapter_cubit.dart`**: Manages the state of the chapters list and handles the fetching of chapter data.
- **`app_provider.dart`**: Manages the global state of the app, such as theme (dark/light mode).

## How It Works

1. **Chapter Data Fetching**: The app uses a `ChapterCubit` to fetch and manage the state of the Surah list. The data is loaded from an API or other data source when the app initializes.
2. **Search Functionality**: Users can type in the search bar, and the list of Surahs is dynamically filtered based on the search query.
3. **Retry Mechanism**: If an error occurs while fetching the data, the user is presented with a retry button that triggers the fetch process again.

<!--
## Screenshots

(Include screenshots here)

## Contributing

Contributions are welcome! If you find any bugs or have feature suggestions, feel free to create an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
-->

