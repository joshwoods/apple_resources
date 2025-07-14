

- SwiftUI
-  LayoutProperties 

Structure

# LayoutProperties

Layout-specific properties of a layout container.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LayoutProperties
```

## Overview

This structure contains configuration information that’s applicable to a layout container. For example, the stackOrientation value indicates the layout’s primary axis, if any.

You can use an instance of this type to characterize a custom layout container, which is a type that conforms to the Layout protocol. Implement the protocol’s layoutProperties property to return an instance. For example, you can indicate that your layout has a vertical stack orientation:

```
extension BasicVStack {
    static var layoutProperties: LayoutProperties {
        var properties = LayoutProperties()
        properties.stackOrientation = .vertical
        return properties
    }
}
```

If you don’t implement the property in your custom layout, the protocol provides a default implementation that returns a `LayoutProperties` instance with default values.

## Topics

### Creating a layout properties instance

init()

Creates a default set of properties.

### Getting layout properties

var stackOrientation: Axis?

The orientation of the containing stack-like container.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring a custom layout

struct ProposedViewSize

A proposal for the size of a view.

struct ViewSpacing

A collection of the geometric spacing preferences of a view.

