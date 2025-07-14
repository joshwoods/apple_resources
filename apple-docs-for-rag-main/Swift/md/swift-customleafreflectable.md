

- Swift
-  CustomLeafReflectable 

Protocol

# CustomLeafReflectable

A type that explicitly supplies its own mirror, but whose descendant classes are not represented in the mirror unless they also override `customMirror`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol CustomLeafReflectable : CustomReflectable
```

## Relationships

### Inherits From

- CustomReflectable

## See Also

### Customizing Your Type’s Reflection

protocol CustomReflectable

A type that explicitly supplies its own mirror.

protocol CustomPlaygroundDisplayConvertible

A type that supplies a custom description for playground logging.

typealias PlaygroundQuickLook

The sum of types that can be used as a Quick Look representation.

macro DebugDescription()

Converts description definitions to a debugger Type Summary.

