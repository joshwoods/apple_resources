

- SwiftUI
- EnvironmentValues
-  headerProminence 

Instance Property

# headerProminence

The prominence to apply to section headers within a view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var headerProminence: Prominence { get set }
```

## Discussion

The default is Prominence.standard.

## See Also

### Configuring headers

func headerProminence(Prominence) -> some View

Sets the header prominence for this view.

enum Prominence

A type indicating the prominence of a view hierarchy.

var defaultMinListHeaderHeight: CGFloat?

The default minimum height of a header in a list.

