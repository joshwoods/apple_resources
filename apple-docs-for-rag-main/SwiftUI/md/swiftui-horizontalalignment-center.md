

- SwiftUI
- HorizontalAlignment
-  center 

Type Property

# center

A guide that marks the horizontal center of the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let center: HorizontalAlignment
```

## Discussion

Use this guide to align the centers of views:

The following code generates the image above using a VStack:

```
struct HorizontalAlignmentCenter: View {
    var body: some View {
        VStack(alignment: .center, spacing: 0) {
            Color.red.frame(width: 1)
            Text("Center").font(.title).border(.gray)
            Color.red.frame(width: 1)
        }
    }
}
```

## See Also

### Getting guides

static let leading: HorizontalAlignment

A guide that marks the leading edge of the view.

static let trailing: HorizontalAlignment

A guide that marks the trailing edge of the view.

static let listRowSeparatorLeading: HorizontalAlignment

A guide marking the leading edge of a `List` row separator.

static let listRowSeparatorTrailing: HorizontalAlignment

A guide marking the trailing edge of a `List` row separator.

