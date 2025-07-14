

- SwiftUI
- VerticalAlignment
-  lastTextBaseline 

Type Property

# lastTextBaseline

A guide that marks the bottom-most text baseline in a view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let lastTextBaseline: VerticalAlignment
```

## Discussion

Use this guide to align with the baseline of the bottom-most text in a view. The guide aligns with the bottom of a view that contains no text.

The following code generates the image above using an HStack:

```
struct VerticalAlignmentLastTextBaseline: View {
    var body: some View {
        HStack(alignment: .lastTextBaseline, spacing: 0) {
            Color.red.frame(height: 1)
            Text("Last Text Baseline").font(.title).border(.gray)
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

static let bottom: VerticalAlignment

A guide that marks the bottom edge of the view.

static let firstTextBaseline: VerticalAlignment

A guide that marks the top-most text baseline in a view.

