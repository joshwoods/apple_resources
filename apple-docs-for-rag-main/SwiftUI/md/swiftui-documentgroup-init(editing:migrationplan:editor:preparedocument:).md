

- SwiftUI
- DocumentGroup
-  init(editing:migrationPlan:editor:prepareDocument:) 

Initializer

# init(editing:migrationPlan:editor:prepareDocument:)

Instantiates a document group for creating and editing documents described by the last `Schema` in the migration plan.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
init(
    editing contentType: UTType,
    migrationPlan: any SchemaMigrationPlan.Type,
    editor: @escaping () -> Content,
    prepareDocument: @escaping (ModelContext) -> Void = { _ in }
)
```

Available when `Document` is `ModelDocument` and `Content` conforms to `View`.

## Parameters 

`editing`  

The content type of the document. It should conform to `UTType.package`.

`migrationPlan`  

The description of steps required to migrate older document versions so that they can be opened and edited. The last `VersionedSchema` in the plan is considered to be the current application schema.

`editor`  

The editing UI for the provided document.

## See Also

### Editing a document backed by a persistent store

init(editing:contentType:editor:prepareDocument:)

Instantiates a document group for creating and editing documents that store a specific model type.

