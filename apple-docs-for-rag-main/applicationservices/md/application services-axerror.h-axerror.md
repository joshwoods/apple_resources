

- Application Services
- AXError.h
-  AXError 

Enumeration

# AXError

Error codes returned by accessibility functions.

macOS 10.2+

``` source
enum AXError : Int32, @unchecked Sendable
```

## Topics

### Enumeration Cases

case apiDisabled

Assistive applications are not enabled in System Preferences.

case actionUnsupported

The referenced action is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case attributeUnsupported

The referenced attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case cannotComplete

A fundamental error has occurred, such as a failure to allocate memory during processing.

case failure

case illegalArgument

The value received in this event is an invalid value for this attribute. This also applies for invalid parameters in parameterized attributes.

case invalidUIElement

The accessibility object received in this event is invalid.

case invalidUIElementObserver

The observer for the accessibility object received in this event is invalid.

case noValue

case notEnoughPrecision

case notImplemented

case notificationAlreadyRegistered

case notificationNotRegistered

case notificationUnsupported

case parameterizedAttributeUnsupported

The parameterized attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case success

## Relationships

### Conforms To

- Sendable

