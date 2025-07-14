

- SwiftUI
-  EditButton 

Structure

# EditButton

A button that toggles the edit mode environment value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
struct EditButton
```

## Overview

An edit button toggles the environment’s editMode value for content within a container that supports edit mode. In the following example, an edit button placed inside a NavigationView supports editing of a List:

```
@State private var fruits = [
    "Apple",
    "Banana",
    "Papaya",
    "Mango"
]

var body: some View {
    NavigationView {
        List {
            ForEach(fruits, id: \.self) { fruit in
                Text(fruit)
            }
            .onDelete { fruits.remove(atOffsets: $0) }
            .onMove { fruits.move(fromOffsets: $0, toOffset: $1) }
        }
        .navigationTitle("Fruits")
        .toolbar {
            EditButton()
        }
    }
}
```

Because the ForEach in the above example defines behaviors for onDelete(perform:) and onMove(perform:), the editable list displays the delete and move UI when the user taps Edit. Notice that the Edit button displays the title “Done” while edit mode is active:

You can also create custom views that react to changes in the edit mode state, as described in EditMode.

## Topics

### Creating an edit button

init()

Creates an Edit button instance.

## Relationships

### Conforms To

- View

## See Also

### Creating special-purpose buttons

struct PasteButton

A system button that reads items from the pasteboard and delivers it to a closure.

struct RenameButton

A button that triggers a standard rename action.

