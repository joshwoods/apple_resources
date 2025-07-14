

- SwiftUI
- VerticalAlignment
-  top 

Type Property

# top

A guide that marks the top edge of the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let top: VerticalAlignment
```

## Mentioned in 

Laying out a simple view

## Discussion

Use this guide to align the top edges of views:

The following code generates the image above using an HStack:

```
struct VerticalAlignmentTop: View {
    var body: some View {
        HStack(alignment: .top, spacing: 0) {
            Color.red.frame(height: 1)
            Text("Top").font(.title).border(.gray)
            Color.red.frame(height: 1)
        }
    }
}
```

## See Also

### Getting guides

static let center: VerticalAlignment

A guide that marks the vertical center of the view.

static let bottom: VerticalAlignment

A guide that marks the bottom edge of the view.

static let firstTextBaseline: VerticalAlignment

A guide that marks the top-most text baseline in a view.

static let lastTextBaseline: VerticalAlignment

A guide that marks the bottom-most text baseline in a view.

