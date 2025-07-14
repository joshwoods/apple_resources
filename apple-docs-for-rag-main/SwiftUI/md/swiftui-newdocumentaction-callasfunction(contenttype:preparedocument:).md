

- SwiftUI
- NewDocumentAction
-  callAsFunction(contentType:prepareDocument:) 

Instance Method

# callAsFunction(contentType:prepareDocument:)

Presents a new document window with preset contents.

SwiftDataSwiftUImacOS 14.0+

``` source
@MainActor @preconcurrency
func callAsFunction(
    contentType: UTType,
    prepareDocument: @escaping (ModelContext) -> Void
)
```

## Parameters 

`contentType`  

The content type of the document.

`prepareDocument`  

The closure that accepts `ModelContext` associated with the new document. Use this closure to set the document’s initial contents before it is displayed: insert preconfigured models in the provided `ModelContext`.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the newDocument action.

For example, a Todo app might have a way to create a sample prepopulated Todo list as a part of onboarding experience:

```
newDocument(contentType: .todoList) { modelContext in
    let todoList = TodoList(
        title: "🎬 Movie night",
        items: [
            TodoItem(title: "🍿 Buy popcorn"),
            TodoItem(title: "🍨 Make some ice cream",
            TodoItem(title: "💡 Hang a string of lights")
        ]
    )
    modelContext.insert(todoList)
}
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(_:)

Presents a new document window.

func callAsFunction(contentType: UTType)

Presents a new document window.

