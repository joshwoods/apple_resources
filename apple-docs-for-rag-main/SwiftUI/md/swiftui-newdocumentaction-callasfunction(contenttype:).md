

- SwiftUI
- NewDocumentAction
-  callAsFunction(contentType:) 

Instance Method

# callAsFunction(contentType:)

Presents a new document window.

macOS 14.0+

``` source
@MainActor @preconcurrency
func callAsFunction(contentType: UTType)
```

## Parameters 

`contentType`  

The content type of the document.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the newDocument action:

```
newDocument(contentType: .todoList)

 extension UTType {
     static var todoList = UTType(exportedAs: "com.myApp.todoList")
 }
```

Important

If your app declares custom uniform type identifiers, include corresponding entries in the app’s `Info.plist` file. For more information, see Defining file and data types for your app. Also, remember to specify the supported Document types in the `Info.plist` file as well.

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(_:)

Presents a new document window.

func callAsFunction(contentType: UTType, prepareDocument: (ModelContext) -> Void)

Presents a new document window with preset contents.

