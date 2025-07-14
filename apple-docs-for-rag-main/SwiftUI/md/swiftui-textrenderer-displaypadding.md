

- SwiftUI
- TextRenderer
-  displayPadding 

Instance Property

# displayPadding

Returns the size of the extra padding added to any drawing layer used to rasterize the text. For example when drawing the text with a shadow this may be used to extend the drawing bounds to avoid clipping the shadow.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var displayPadding: EdgeInsets { get }
```

**Required** Default implementation provided.

## Discussion

The default implementation of this function returns an empty set of insets.

## Default Implementations

### TextRenderer Implementations

var displayPadding: EdgeInsets

Returns the size of the extra padding added to any drawing layer used to rasterize the text. For example when drawing the text with a shadow this may be used to extend the drawing bounds to avoid clipping the shadow.

