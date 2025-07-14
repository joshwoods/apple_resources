

- SwiftUI
- EnvironmentValues
-  defaultMinListHeaderHeight 

Instance Property

# defaultMinListHeaderHeight

The default minimum height of a header in a list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var defaultMinListHeaderHeight: CGFloat? { get set }
```

## Discussion

When this value is `nil`, the system chooses the appropriate height. The default is `nil`.

## See Also

### Configuring headers

func headerProminence(Prominence) -> some View

Sets the header prominence for this view.

var headerProminence: Prominence

The prominence to apply to section headers within a view.

enum Prominence

A type indicating the prominence of a view hierarchy.

