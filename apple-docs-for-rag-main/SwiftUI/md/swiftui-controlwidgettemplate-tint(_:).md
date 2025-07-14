

- SwiftUI
- ControlWidgetTemplate
-  tint(\_:) 

Instance Method

# tint(\_:)

Sets the tint color within this control widget template.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func tint(_ tint: Color?) -> some ControlWidgetTemplate
```

## Parameters 

`tint`  

The tint Color to apply.

## Discussion

Controls do not respect the tint(_:) modifier when applied to control labels, nor do controls support arbitrary tint shape styles. Instead, define a tint color for your control by applying this modifier to its template:

```
struct GarageDoorOpener: ControlWidget {
    var body: some ControlWidgetConfiguration {
        StaticControlConfiguration(...) {
            ControlWidgetToggle(...) {
                Label(
                    $0 ? "Open" : "Closed",
                    systemImage: $0 ? "door.open" : "door.closed"
                )
            }
            .tint(.orange)
        }
    }
}
```

