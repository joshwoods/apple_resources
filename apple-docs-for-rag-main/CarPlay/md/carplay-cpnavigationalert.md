

- CarPlay
-  CPNavigationAlert 

Class

# CPNavigationAlert

An alert that displays map- or navigation-related information to the user.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPNavigationAlert
```

## Overview

To display a navigation alert, create an instance of CPNavigationAlert and pass it to the map template’s present(navigationAlert:animated:) method. When creating an alert, you must provide a title, action, and duration. The duration tells the system how long to show the alert before automatically dismissing it. You can also include a subtitle and secondary action when needed.

The system displays the primary and secondary actions as buttons on the alert. After the user taps the button, the system calls the action’s handler block, which is where your app performs the requested action. The system also dismisses the alert after the user taps the button. However, your app can dismiss the alert without any user interaction by calling dismissNavigationAlert(animated:completion:).

## Topics

### Creating a Navigation Alert

init(titleVariants: [String], subtitleVariants: [String]?, image: UIImage?, primaryAction: CPAlertAction, secondaryAction: CPAlertAction?, duration: TimeInterval)

Creates a navigation alert.

init(titleVariants: [String], subtitleVariants: [String]?, imageSet: CPImageSet?, primaryAction: CPAlertAction, secondaryAction: CPAlertAction?, duration: TimeInterval)

Creates a navigation alert.

Deprecated

### Getting Titles

var titleVariants: [String]

An array of title strings.

var subtitleVariants: [String]

An array of subtitle strings.

func updateTitleVariants([String], subtitleVariants: [String])

Updates title and subtitle variants.

### Getting the Alert Image

var image: UIImage?

An image displayed in the navigation alert.

var imageSet: CPImageSet?

An image set displayed in the navigation alert.

### Getting the Actions

var primaryAction: CPAlertAction

The primary action, and button, for the navigation alert.

var secondaryAction: CPAlertAction?

An optional secondary action, and button, for the navigation alert.

### Getting the Alert Duration

var duration: TimeInterval

The amount of time, in seconds, that the alert is visible.

let CPNavigationAlertMinimumDuration: TimeInterval

A constant that defines the minimum amount of time that an alert is visible.

### Enumerations

enum DismissalContext

A set of reasons for dismissing a navigation alert.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Displaying a Navigation Alert

func present(navigationAlert: CPNavigationAlert, animated: Bool)

Displays a navigation alert on the map template.

func dismissNavigationAlert(animated: Bool, completion: (Bool) -> Void)

Tells the map template to dismiss the visable navigation alert.

var currentNavigationAlert: CPNavigationAlert?

The visible navigation alert.

