

- SwiftUI
- View
-  importsItemProviders(\_:onImport:) 

Instance Method

# importsItemProviders(\_:onImport:)

Enables importing item providers from services, such as Continuity Camera on macOS.

macOS 12.0+

``` source
nonisolated
func importsItemProviders(
    _ contentTypes: [UTType],
    onImport: @escaping ([NSItemProvider]) -> Bool
) -> some View
```

## Parameters 

`contentTypes`  

The types of content that the view supports importing. An empty array means the view does not currently support importing.

`onImport`  

A closure that will be called with the imported service item. Return `false` to indicate that there was a failure to receive the items.

## See Also

### Importing and exporting using item providers

func exportsItemProviders([UTType], onExport: () -> [NSItemProvider]) -> some View

Exports a read-only item provider for consumption by shortcuts, quick actions, and services.

func exportsItemProviders([UTType], onExport: () -> [NSItemProvider], onEdit: ([NSItemProvider]) -> Bool) -> some View

Exports a read-write item provider for consumption by shortcuts, quick actions, and services.

