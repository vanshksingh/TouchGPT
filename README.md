

# TouchBarController

![IMG_3869](https://github.com/vanshksingh/TouchGPT/assets/114809624/03fab4f5-99c5-4243-bd4d-e3345a9cf012)

## Demo Link
https://www.reddit.com/r/MacOS/s/WWlvcRv61G

## Description

`TouchBarController` is a class in Swift that manages an `NSTouchBar` instance, allowing you to control the Touch Bar functionality in macOS applications. The controller uses `NSTouchBarDelegate` protocol methods to manage and customize the Touch Bar.

## Features

- **Singleton Instance**: `TouchBarController.shared` provides a singleton instance of the `TouchBarController` class.
- **Touch Bar Management**: The class manages the Touch Bar, including presentation and dismissal.
- **Refresh**: The `refresh` function refreshes the Touch Bar, removing the existing Touch Bar and creating a new one.
- **Control Strip Presence**: The `setupControlStripPresence` function sets up the control strip presence for the Touch Bar.
- **Present and Dismiss**: The class provides methods to present and dismiss the Touch Bar.
- **Touch Bar Items**: The `touchBar` method in the class delegates the creation of touch bar items based on their identifier.

## Usage

1. **Initialization**:
    - The `TouchBarController` class uses the singleton pattern and is initialized with the `TouchBarController.shared` property.

2. **Setting Up the Touch Bar**:
    - Call `TouchBarController.shared.setupControlStripPresence()` to set up the control strip presence for the Touch Bar.

3. **Presenting the Touch Bar**:
    - Use `TouchBarController.shared.presentTouchBar()` to present the Touch Bar.

4. **Dismissing the Touch Bar**:
    - Use `TouchBarController.shared.dismissTouchBar()` to dismiss the Touch Bar.

5. **Refreshing the Touch Bar**:
    - Call `TouchBarController.shared.refresh()` to refresh the Touch Bar.

## Customization

You can customize the Touch Bar items by providing different item identifiers and creating instances of `NSTouchBarItem` with custom views and actions.

- Use `touchBar` method to create custom items for the Touch Bar based on the specified identifier.

## Dependencies

- Cocoa
- AppKit

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request.

