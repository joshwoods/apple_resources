

- SwiftUI
- WidgetBundle
-  body 

Instance Property

# body

Declares the group of widgets that an app supports.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
@WidgetBundleBuilder @MainActor @preconcurrency
var body: Self.Body { get }
```

**Required**

## Discussion

The order that the widgets appear in this property determines the order they are shown to the user when adding a widget. The following example shows how to use a widget bundle builder to define a body showing a game status widget first and a character detail widget second:

```
@main
struct GameWidgets: WidgetBundle {
   var body: some Widget {
       GameStatusWidget()
       CharacterDetailWidget()
   }
}
```

## See Also

### Implementing a widget bundle

associatedtype Body : Widget

The type of widget that represents the content of the bundle.

**Required**

struct WidgetBundleBuilder

A custom attribute that constructs a widget bundle’s body.

