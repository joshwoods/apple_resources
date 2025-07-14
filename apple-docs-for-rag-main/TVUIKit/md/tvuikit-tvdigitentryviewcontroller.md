

- TVUIKit
-  TVDigitEntryViewController 

Class

# TVDigitEntryViewController

A view controller that enables the user to enter digits, like a passcode, in your app.

tvOS 12.0+

``` source
@MainActor
class TVDigitEntryViewController
```

## Overview

Use the `TVDigitEntryViewController` class to manage a digit entry view. The digit entry view is automatically presented by the view controller and consists of boxes that display digits and a digit keyboard.

## Topics

### Configuring the Digit Entry View

var numberOfDigits: Int

The number of required digits.

var titleText: String?

The title of the digit entry view.

var promptText: String?

A prompt that displays any additional required information.

var isSecureDigitEntry: Bool

A Boolean value that indicates whether an entered digit is immediately obscured.

### Entering Information

var entryCompletionHandler: (String) -> Void

A completion handler that cues the app that the user has entered the required number of digits for the digit entry view.

func clearEntry(animated: Bool)

Removes all digits from the digit entry view.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

