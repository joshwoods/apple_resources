

- CarPlay
-  CPActionSheetTemplate 

Class

# CPActionSheetTemplate

A template that displays a modal action sheet.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPActionSheetTemplate
```

## Overview

You must present action sheets modally by calling the presentTemplate(_:animated:completion:) method available on your app’s instance of CPInterfaceController. The user dismisses the action sheet by pressing a button, or you can dismiss it by calling the interface controller’s dismissTemplate(animated:completion:) method.

## Topics

### Creating an Action Sheet Template

init(title: String?, message: String?, actions: [CPAlertAction])

Creates an action sheet template.

### Getting Action Sheet Template Information

var title: String?

The title of the action sheet.

var message: String?

The descriptive message providing details about the reason for displaying the action sheet.

var actions: [CPAlertAction]

The list of actions available on the action sheet.

## Relationships

### Inherits From

- CPTemplate

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

### Actions and Alerts

class CPAlertTemplate

A template that displays a modal alert.

class CPAlertAction

An object that encapsulates an action the user can perform on an action sheet or alert.

