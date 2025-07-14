

- SwiftUI
- HorizontalAlignment
-  trailing 

Type Property

# trailing

A guide that marks the trailing edge of the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let trailing: HorizontalAlignment
```

## Discussion

Use this guide to align the trailing edges of views. For a device that uses a left-to-right language, the trailing edge is on the right:

The following code generates the image above using a VStack:

```
struct HorizontalAlignmentTrailing: View {
    var body: some View {
        VStack(alignment: .trailing, spacing: 0) {
            Color.red.frame(width: 1)
            Text("Trailing").font(.title).border(.gray)
            Color.red.frame(width: 1)
        }
    }
}
```

## See Also

### Getting guides

static let leading: HorizontalAlignment

A guide that marks the leading edge of the view.

static let center: HorizontalAlignment

A guide that marks the horizontal center of the view.

static let listRowSeparatorLeading: HorizontalAlignment

A guide marking the leading edge of a `List` row separator.

static let listRowSeparatorTrailing: HorizontalAlignment

A guide marking the trailing edge of a `List` row separator.

