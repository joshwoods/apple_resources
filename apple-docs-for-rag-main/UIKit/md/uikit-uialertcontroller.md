

- UIKit
-  UIAlertController 

Class

# UIAlertController

An object that displays an alert message.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIAlertController
```

## Mentioned in 

Getting the user’s attention with alerts and action sheets

## Overview

Use this class to configure alerts and action sheets with the message that you want to display and the actions from which to choose. After configuring the alert controller with the actions and style you want, present it using the present(_:animated:completion:) method. UIKit displays alerts and action sheets modally over your app’s content.

In addition to displaying a message to a user, you can associate actions with your alert controller to give people a way to respond. For each action you add using the addAction(_:) method, the alert controller configures a button with the action details. When a person taps that action, the alert controller executes the block you provided when creating the action object. The following code shows how to configure an alert with a single action.

- Swift
- Objective-C

```
let alert = UIAlertController(title: "My Alert", message: "This is an alert.", preferredStyle: .alert) 
alert.addAction(UIAlertAction(title: NSLocalizedString("OK", comment: "Default action"), style: .default, handler: { _ in 
NSLog("The \"OK\" alert occured.")
}))
self.present(alert, animated: true, completion: nil)
```

```
UIAlertController* alert = [UIAlertController alertControllerWithTitle:@"My Alert"
                               message:@"This is an alert."
                               preferredStyle:UIAlertControllerStyleAlert];

UIAlertAction* defaultAction = [UIAlertAction actionWithTitle:@"OK" style:UIAlertActionStyleDefault
   handler:^(UIAlertAction * action) {}];

[alert addAction:defaultAction];
[self presentViewController:alert animated:YES completion:nil];
```

When configuring an alert with the UIAlertController.Style.alert style, you can also add text fields to the alert interface. The alert controller lets you provide a block for configuring your text fields prior to display. The alert controller maintains a reference to each text field so that you can access its value later.

Important

The UIAlertController class is intended to be used as-is and doesn’t support subclassing. The view hierarchy for this class is private and must not be modified.

## Topics

### Creating an alert controller

convenience init(title: String?, message: String?, preferredStyle: UIAlertController.Style)

Creates and returns a view controller for displaying an alert.

### Configuring the alert

var title: String?

The title of the alert.

var message: String?

Descriptive text that provides more details about the reason for the alert.

var preferredStyle: UIAlertController.Style

The style of the alert controller.

### Configuring the user actions

func addAction(UIAlertAction)

Attaches an action object to the alert or action sheet.

var actions: [UIAlertAction]

The actions that the user can take in response to the alert or action sheet.

var preferredAction: UIAlertAction?

The preferred action for the user to take from an alert.

### Configuring text fields

func addTextField(configurationHandler: ((UITextField) -> Void)?)

Adds a text field to an alert.

var textFields: [UITextField]?

The array of text fields displayed by the alert.

### Configuring alert severity

var severity: UIAlertControllerSeverity

Indicates the severity of the alert.

enum UIAlertControllerSeverity

Constants for specifying the severity of an alert in apps built with Mac Catalyst.

### Constants

enum Style

Constants indicating the type of alert to display.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UISpringLoadedInteractionSupporting
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Alerts

Getting the user’s attention with alerts and action sheets

Present important information to the user or prompt the user about an important choice.

class UIAlertAction

An action that can be taken when the user taps a button in an alert.

