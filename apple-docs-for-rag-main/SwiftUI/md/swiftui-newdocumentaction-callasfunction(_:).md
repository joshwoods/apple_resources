

- SwiftUI
- NewDocumentAction
-  callAsFunction(\_:) 

Instance Method

# callAsFunction(\_:)

Presents a new document window.

macOS 13.0+

``` source
@MainActor @preconcurrency
func callAsFunction(_ newDocument: @autoclosure @escaping () -> D) where D : FileDocument
```

Show all declarations

## Parameters 

`newDocument`  

The new file document to present.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the newDocument action:

```
newDocument(TextDocument(text: selectedText))
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(contentType: UTType)

Presents a new document window.

func callAsFunction(contentType: UTType, prepareDocument: (ModelContext) -> Void)

Presents a new document window with preset contents.

