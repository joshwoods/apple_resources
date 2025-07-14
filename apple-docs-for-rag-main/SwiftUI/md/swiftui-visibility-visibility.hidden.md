

- SwiftUI
- Visibility
-  Visibility.hidden 

Case

# Visibility.hidden

The element may be hidden.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case hidden
```

## Discussion

Some APIs may use this value to represent a hint or preference, rather than a mandatory assertion. For example, setting confirmation dialog title visibility to `hidden` using the confirmationDialog(_:isPresented:titleVisibility:actions:) modifier may not always hide the dialog title, which is required on some platforms.

## See Also

### Getting visibility options

case automatic

The element may be visible or hidden depending on the policies of the component accepting the visibility configuration.

case visible

The element may be visible.

