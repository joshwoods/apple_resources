

- SwiftUI
- TextSelectability
-  disabled 

Type Property

# disabled

A selectability value that disables text selection by the person using your app.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static var disabled: DisabledTextSelectability { get }
```

Available when `Self` is `DisabledTextSelectability`.

## Discussion

Use this property to disable text selection of views that you don’t want people to select and copy, even if contained within an overall context that allows text selection.

```
content // Content that might contain Text views.
   .textSelection(.disabled)
   .padding()
   .contentShape(Rectangle())
   .gesture(someGesture)
```

## See Also

### Getting selectability options

static var enabled: EnabledTextSelectability

A selectability value that enables text selection by a person using your app.

