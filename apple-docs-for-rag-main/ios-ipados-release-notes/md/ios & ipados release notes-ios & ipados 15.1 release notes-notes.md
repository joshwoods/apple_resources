

- iOS &amp; iPadOS Release Notes
-  iOS & iPadOS 15.1 Release Notes 

Article

# iOS & iPadOS 15.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The iOS & iPadOS 15 SDK provides support to develop apps for iPhone, iPad, and iPod touch devices running iOS & iPadOS 15.1. The SDK comes bundled with Xcode 13, available from the Mac App Store. For information on the compatibility requirements for Xcode 13, see Xcode 13 Release Notes.

### CoreData

#### Known Issues

- `NSExpression` immediately forbids certain operations that have significant side effects, like creating and destroying objects. Additionally, casting string class names into Class objects with `NSConstantValueExpression` is deprecated. (84017178)

  **Workaround:** Pass temporary objects to `NSExpression` in the context parameter of expressionValueWithObject:context:, or with `NSPredicate` as the `substitutionVariables` parameter of evaluateWithObject:substitutionVariables:. You can create a derived predicate with all the substitution variables replaced (bound), using withSubstitutionVariables(_:) on an existing `NSPredicate` so that code using the object can continue to use a simple `evaluate(with object: Any?)` invocation.

### Home

#### Known Issues

- The query for the connected admin list isn’t supported by Matter accessories. (82398328)

- Matter accessory notifications don’t work. (82634464)

  **Workaround:** Relaunch the Home app to force a refresh of the Matter accessory state.

### SharePlay

#### New Features

- SharePlay is now available in iOS 15.1, iPadOS 15.1, and tvOS 15.1. You can submit your apps that support SharePlay now. It’s also enabled in macOS 12.1 beta, so you can build SharePlay experiences across Apple platforms using the Group Activities entitlement, without the need for the SharePlay Development Profile.

### SwiftUI

#### Known Issues

- The BorderedButtonStyle no longer has a default hover effect.

  **Workaround:** Use the HoverEffect modifier on the Button. (81759097)

### Telephony

#### Known Issues

- Users might experience loss of audio during calls, followed by the call being dropped in some conditions. (83381816)

  **Workaround:** Toggle Airplane Mode on and off, or reboot.

### VoiceOver

#### Resolved Issues

- Alarms now activate correctly in the Clock app. (82968832)

## See Also

### iOS &amp; iPadOS 15

iOS & iPadOS 15.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15 Release Notes

Update your apps to use new features, and test your apps against API changes.

