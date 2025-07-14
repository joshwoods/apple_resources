

- Application Services
- AXError.h
- AXError
-  AXError.parameterizedAttributeUnsupported 

Enumeration Case

# AXError.parameterizedAttributeUnsupported

The parameterized attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

macOS 10.3+

``` source
case parameterizedAttributeUnsupported = -25213
```

## See Also

### Result Codes

case illegalArgument

The value received in this event is an invalid value for this attribute. This also applies for invalid parameters in parameterized attributes.

case invalidUIElement

The accessibility object received in this event is invalid.

case invalidUIElementObserver

The observer for the accessibility object received in this event is invalid.

case cannotComplete

A fundamental error has occurred, such as a failure to allocate memory during processing.

case attributeUnsupported

The referenced attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case actionUnsupported

The referenced action is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case apiDisabled

Assistive applications are not enabled in System Preferences.

