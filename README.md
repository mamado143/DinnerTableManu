# Menu App

This repository contains an Android application that displays a menu of products. Users can view the products, filter them by category, and sort them based on different criteria.

## Getting Started

To get started with the Menu App, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/menu-app.git`
2. Open the project in Android Studio.
3. Build and run the app on an Android device or emulator.

## Features

The Menu App has the following features:

- Displaying a grid of products.
- Starting a detailed product activity when a product is selected.
- Sorting products based on different criteria (alphabetically, price ascending, price descending).
- Filtering products by category (all, drinks, food, dessert).

## Usage

When the app is launched, it will display a grid of products. You can tap on a product to view its details in a separate activity.

To sort the products, click on the sorting menu icon in the toolbar. A dropdown menu will appear with sorting options. Select an option to sort the products accordingly.

To filter the products, click on the filter menu icon in the toolbar. A dropdown menu will appear with filter options. Select an option to filter the products by category.

## Code Structure

The main entry point of the app is the `MainActivity` class, located in the `com.littlelemon.menu` package. It sets up the UI and handles user interactions.

The UI is built using Jetpack Compose, and the UI composition logic is encapsulated in the `InitUI` composable function.

The `ProductsGrid` composable function displays the grid of products, and it takes a list of products as input. It also receives a callback function, `startProductActivity`, which is triggered when a product is selected.

The `ProductActivity` class is responsible for displaying the detailed view of a product. It receives the product information through an intent extra.

The `SortHelper` and `FilterHelper` classes provide utility methods for sorting and filtering the products, respectively.
## Dependencies

The Menu App relies on the following dependencies:

- `androidx.activity:activity-compose`: Provides support for Compose UI in an Android activity.
- `androidx.compose.runtime:runtime-livedata`: Enables using LiveData with Compose.
- `androidx.core:core-ktx`: Provides core Kotlin extensions for Android.
- `androidx.lifecycle:lifecycle-runtime-ktx`: Provides lifecycle-related functionalities.
- `androidx.appcompat:appcompat`: Provides compatibility for using the latest features on older Android versions.
- `androidx.compose.ui:ui-tooling`: Provides UI tooling support for Compose.
- `androidx.compose.material:material`: Provides Material Design components for Compose UI.

## Project Structure

The project follows a standard Android project structure. Here is an overview of the main directories and files:

- `app/src/main/java/com/littlelemon/menu`: Contains the main source code of the app.
  - `MainActivity.kt`: The entry point of the app that sets up the UI and handles user interactions.
  - `ProductActivity.kt`: Activity for displaying detailed product information.
  - `ProductsGrid.kt`: Composable function for displaying the grid of products.
  - `Products.kt`: Data class representing a list of products.
  - `SortHelper.kt`: Helper class for sorting products.
  - `FilterHelper.kt`: Helper class for filtering products.
- `app/src/main/res`: Contains the Android resource files.
  - `layout/activity_main.xml`: XML layout file for the main activity.
  - `menu/products_menu.xml`: XML menu file for the toolbar menu.
  - `mipmap`: Directory for app launcher icons.
  - `values`: Directory for various resource files (e.g., colors, strings, styles).

## Testing

The Menu App currently does not have any automated tests. Adding tests is highly recommended to ensure the stability and correctness of the application. You can add unit tests using frameworks like JUnit or instrumented tests using frameworks like Espresso.

## Support and Issues

If you encounter any issues or have any questions or suggestions regarding the Menu App, please [open an issue](https://github.com/your-username/menu-app/issues) on the GitHub repository. We appreciate your feedback and will do our best to address any concerns.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code according to your needs. Make sure to comply with the license terms when distributing or using the project.

