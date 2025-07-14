

- SwiftUI
- Visibility
-  Visibility.visible 

Case

# Visibility.visible

The element may be visible.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case visible
```

## Discussion

Some APIs may use this value to represent a hint or preference, rather than a mandatory assertion. For example, setting list row separator visibility to `visible` using the listRowSeparator(_:edges:) modifier may not always result in any visible separators, especially for list styles that do not include separators as part of their design.

## See Also

### Getting visibility options

case automatic

The element may be visible or hidden depending on the policies of the component accepting the visibility configuration.

case hidden

The element may be hidden.

