

- SwiftUI
- VerticalAlignment
-  bottom 

Type Property

# bottom

A guide that marks the bottom edge of the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let bottom: VerticalAlignment
```

## Mentioned in 

Aligning views within a stack

## Discussion

Use this guide to align the bottom edges of views:

The following code generates the image above using an HStack:

```
struct VerticalAlignmentBottom: View {
    var body: some View {
        HStack(alignment: .bottom, spacing: 0) {
            Color.red.frame(height: 1)
            Text("Bottom").font(.title).border(.gray)
            Color.red.frame(height: 1)
        }
    }
}
```

## See Also

### Getting guides

static let top: VerticalAlignment

A guide that marks the top edge of the view.

static let center: VerticalAlignment

A guide that marks the vertical center of the view.

static let firstTextBaseline: VerticalAlignment

A guide that marks the top-most text baseline in a view.

static let lastTextBaseline: VerticalAlignment

A guide that marks the bottom-most text baseline in a view.

