

- SwiftUI
- DocumentGroup
-  init(viewing:contentType:viewer:) 

Initializer

# init(viewing:contentType:viewer:)

Instantiates a document group for viewing documents that store a specific model type.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
init(
    viewing modelType: any PersistentModel.Type,
    contentType: UTType,
    viewer: @escaping () -> Content
)
```

Available when `Document` is `ModelDocument` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`modelType`  

The model type defining the schema used for each document.

`contentType`  

The content type of document your app can view. It should conform to `UTType.package`.

`viewer`  

The viewing UI for the provided document.

## Discussion

```
 @main
 struct Todo: App {
     var body: some Scene {
         DocumentGroup(viewing: TodoItem.self, contentType: .todoItem) {
             ContentView()
         }
     }
 }

 extension UTType {
     static var todoItem = UTType(exportedAs: "com.myApp.todoItem")
 }
```

Important

If your app declares custom uniform type identifiers, include corresponding entries in the app’s `Info.plist`. For more information, see Defining file and data types for your app. Also, remember to specify the supported Document types in the `Info.plist` as well.

## See Also

### Viewing a document backed by a persistent store

init(viewing: UTType, migrationPlan: any SchemaMigrationPlan.Type, viewer: () -> Content)

Instantiates a document group for viewing documents described by the last `Schema` in the migration plan.

