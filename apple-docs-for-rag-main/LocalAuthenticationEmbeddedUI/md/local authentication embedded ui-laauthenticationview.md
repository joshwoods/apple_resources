

- Local Authentication Embedded UI
-  LAAuthenticationView 

Class

# LAAuthenticationView

A graphical representation of the state of biometric authentication.

macOS 12.0+

``` source
@MainActor
class LAAuthenticationView
```

## Overview

In the view that you use to manage authentication, add a local authentication view as a subview and provide it with an LAContext instance. For example, you can do this in the doc://com.apple.documentation/documentation/appkit/nsviewcontroller/1434405-loadview method of your view controller:

```
```

When the view appears, call the context’s evaluatePolicy(_:localizedReason:reply:) method to initiate the authentication:

```
```

The local authentication view displays an icon that depends on the type of authentication you request, and the types of authentication that the system supports. For example, for a device that supports Touch ID, if you request the LAPolicy.deviceOwnerAuthenticationWithBiometricsOrWatch policy, like in the example above, the view displays the familiar finger print icon:

In the case above, if the user has a connected Apple Watch, that authentication mechanism works as well. If you limit the authentication to the LAPolicy.deviceOwnerAuthenticationWithWatch policy, the icon shows an Apple Watch in profile:

You can include other content around this icon that suits your app. The system also displays a message on the Touch Bar or on the user’s Apple Watch, if appropriate. When the evaluation succeeds, the icon transitions into a checkmark:

If you call the evaluation without first attaching it to a local authentication view, the system shows a standard authentication alert instead.

## Topics

### Creating a local authentication view

init(context: LAContext)

Creates a new authentication icon that reflects the current authentication state.

var context: LAContext

The local authentication context associated with the authentication view.

### Controlling the size of a local authentication view

init(context: LAContext, controlSize: NSControl.ControlSize)

Creates a new authentication icon that reflects the current authentication state, using a specified size.

var controlSize: NSControl.ControlSize

The size of the local authentication view user interface element.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

