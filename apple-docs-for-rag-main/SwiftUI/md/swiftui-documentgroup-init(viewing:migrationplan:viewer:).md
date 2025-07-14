

- SwiftUI
- DocumentGroup
-  init(viewing:migrationPlan:viewer:) 

Initializer

# init(viewing:migrationPlan:viewer:)

Instantiates a document group for viewing documents described by the last `Schema` in the migration plan.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
init(
    viewing contentType: UTType,
    migrationPlan: any SchemaMigrationPlan.Type,
    viewer: @escaping () -> Content
)
```

Available when `Document` is `ModelDocument` and `Content` conforms to `View`.

## Parameters 

`viewing`  

The content type of the document. It should conform to `UTType.package`.

`migrationPlan`  

The description of steps required to migrate older document versions so that they can be opened. The last `VersionedSchema` in the plan is considered to be the current application schema.

`viewer`  

The viewing UI for the provided document.

## See Also

### Viewing a document backed by a persistent store

init(viewing:contentType:viewer:)

Instantiates a document group for viewing documents that store a specific model type.

