

- SwiftUI
- ControlWidgetTemplate
-  disabled(\_:) 

Instance Method

# disabled(\_:)

Determines whether users can interact with this control widget.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func disabled(_ disabled: Bool) -> some ControlWidgetTemplate
```

## Parameters 

`disabled`  

A Boolean value that determines whether users can interact with this control.

## Discussion

Controls also respect the disabled(_:) modifier applied to the control’s label. That modifier only disables the label, however. To disable the control overall, apply this modifier to the control template:

```
struct GarageDoorOpener: ControlWidget {
    var body: some ControlWidgetConfiguration {
        StaticControlConfiguration(
            kind: "com.myapp.garagedooropener",
            provider: DoorValueProvider()
        ) { door in
            ControlWidgetToggle(...) {
                Label(
                    $0 ? "Open" : "Closed",
                    systemImage: $0 ? "door.open" : "door.closed"
                )
            }
            .disabled(door.isSafetyLockEngaged)
        }
    }
}
```

