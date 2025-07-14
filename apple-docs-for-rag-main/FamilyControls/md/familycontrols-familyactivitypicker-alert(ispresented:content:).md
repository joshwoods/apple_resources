

- FamilyControls
- FamilyActivityPicker
-  alert(isPresented:content:) 

Instance Method

# alert(isPresented:content:)

Presents an alert to the user.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func alert(
    isPresented: Binding,
    content: () -> Alert
) -> some View
```

## Parameters 

`isPresented`  

A binding to a Boolean value that determines whether to present the alert that you create in the modifier’s `content` closure. When the user presses or taps OK the system sets `isPresented` to `false` which dismisses the alert.

`content`  

A closure returning the alert to present.

## Discussion

Use this method when you need to show an alert to the user. The example below displays an alert that is shown when the user toggles a Boolean value that controls the presentation of the alert:

```
struct OrderCompleteAlert: View {
    @State private var isPresented = false
    var body: some View {
        Button("Show Alert", action: {
            isPresented = true
        })
        .alert(isPresented: $isPresented) {
            Alert(title: Text("Order Complete"),
                  message: Text("Thank you for shopping with us."),
                  dismissButton: .default(Text("OK")))
        }
    }
}
```

## See Also

### Deprecated View Presentation Modifiers

func actionSheet(isPresented: Binding&lt;Bool>, content: () -> ActionSheet) -> some View

Presents an action sheet when a given condition is true.

func actionSheet&lt;T>(item: Binding&lt;T?>, content: (T) -> ActionSheet) -> some View

Presents an action sheet using the given item as a data source for the sheet’s content.

func alert&lt;Item>(item: Binding&lt;Item?>, content: (Item) -> Alert) -> some View

Presents an alert to the user.

