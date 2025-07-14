

- SwiftUI
- ToolbarItemPlacement
-  keyboard 

Type Property

# keyboard

The item is placed in the keyboard section.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
static let keyboard: ToolbarItemPlacement
```

## Discussion

On iOS, keyboard items are above the software keyboard when present, or at the bottom of the screen when a hardware keyboard is attached.

On macOS, keyboard items will be placed inside the Touch Bar.

A `FocusedValue`can be used to adjust the content of the keyboard bar based on the currently focused view. In the example below, the keyboard bar gains additional buttons only when the appropriate `TextField` is focused.

```
enum Field {
    case suit
    case rank
}

struct KeyboardBarDemo : View {
    @FocusedValue(\.field) var field: Field?

    var body: some View {
        HStack {
            TextField("Suit", text: $suitText)
                .focusedValue(\.field, .suit)
            TextField("Rank", text: $rankText)
                .focusedValue(\.field, .rank)
        }
        .toolbar {
            ToolbarItemGroup(placement: .keyboard) {
                if field == .suit {
                    Button("♣️", action: {})
                    Button("♥️", action: {})
                    Button("♠️", action: {})
                    Button("♦️", action: {})
                }
                DoneButton()
            }
        }
    }
}
```

## See Also

### Getting explicit placement

static var topBarLeading: ToolbarItemPlacement

Places the item in the leading edge of the top bar.

static var topBarTrailing: ToolbarItemPlacement

Places the item in the trailing edge of the top bar.

static let bottomBar: ToolbarItemPlacement

Places the item in the bottom toolbar.

static let bottomOrnament: ToolbarItemPlacement

Places the item in an ornament under the window.

static func accessoryBar&lt;ID>(id: ID) -> ToolbarItemPlacement

Creates a unique accessory bar placement.

