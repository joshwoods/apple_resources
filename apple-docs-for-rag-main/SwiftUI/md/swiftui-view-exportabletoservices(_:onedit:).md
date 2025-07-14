

- SwiftUI
- View
-  exportableToServices(\_:onEdit:) 

Instance Method

# exportableToServices(\_:onEdit:)

Exports read-write items for consumption by shortcuts, quick actions, and services.

macOS 13.0+

``` source
nonisolated
func exportableToServices(
    _ payload: @autoclosure @escaping () -> [T],
    onEdit: @escaping ([T]) -> Bool
) -> some View where T : Transferable
```

## Parameters 

`payload`  

A closure that will be called on request of the items by the shortcut or service.

`onEdit`  

A closure that will be called after the shortcut or service completes with its output data. This should replace the selected subpart that was exported with `onExport`. Return `false` to indicate that there was a failure to receive the items.

## Discussion

If the associated view supports selection, the exported item should reflect that selected subpart.

```
@State private var title: String
var body: some View {
    Color.pink
        .frame(width: 400, height: 400)
        .exportableToServices([title]) { editedTitles
            title = editedTitles.first ?? title
            return !editedTitles.isEmpty
        }
}
```

## See Also

### Importing and exporting transferable items

func importableFromServices&lt;T>(for: T.Type, action: ([T]) -> Bool) -> some View

Enables importing items from services, such as Continuity Camera on macOS.

func exportableToServices&lt;T>(@autoclosure () -> [T]) -> some View

Exports items for consumption by shortcuts, quick actions, and services.

