

- SwiftUI
- View
-  exportsItemProviders(\_:onExport:) 

Instance Method

# exportsItemProviders(\_:onExport:)

Exports a read-only item provider for consumption by shortcuts, quick actions, and services.

macOS 12.0+

``` source
nonisolated
func exportsItemProviders(
    _ contentTypes: [UTType],
    onExport: @escaping () -> [NSItemProvider]
) -> some View
```

## Parameters 

`contentTypes`  

The types of content that the view supports exporting. An empty array means the view does not currently support exporting.

`onExport`  

A closure that will be called on request of the items by the shortcut or service.

## Discussion

If the associated view supports selection, the exported item should reflect that selected subpart.

## See Also

### Importing and exporting using item providers

func importsItemProviders([UTType], onImport: ([NSItemProvider]) -> Bool) -> some View

Enables importing item providers from services, such as Continuity Camera on macOS.

func exportsItemProviders([UTType], onExport: () -> [NSItemProvider], onEdit: ([NSItemProvider]) -> Bool) -> some View

Exports a read-write item provider for consumption by shortcuts, quick actions, and services.

