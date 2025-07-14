

- Application Services
- AXError.h
- AXError
-  AXError.cannotComplete 

Enumeration Case

# AXError.cannotComplete

A fundamental error has occurred, such as a failure to allocate memory during processing.

macOS 10.2+

``` source
case cannotComplete = -25204
```

## See Also

### Result Codes

case illegalArgument

The value received in this event is an invalid value for this attribute. This also applies for invalid parameters in parameterized attributes.

case invalidUIElement

The accessibility object received in this event is invalid.

case invalidUIElementObserver

The observer for the accessibility object received in this event is invalid.

case attributeUnsupported

The referenced attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case actionUnsupported

The referenced action is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case apiDisabled

Assistive applications are not enabled in System Preferences.

case parameterizedAttributeUnsupported

The parameterized attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

