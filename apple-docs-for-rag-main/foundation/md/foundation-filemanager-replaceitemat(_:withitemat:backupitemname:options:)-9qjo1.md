

- Foundation
- FileManager
-  replaceItemAt(\_:withItemAt:backupItemName:options:) 

Instance Method

# replaceItemAt(\_:withItemAt:backupItemName:options:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceItemAt(
    _ originalItemURL: URL,
    withItemAt newItemURL: URL,
    backupItemName: String? = nil,
    options: FileManager.ItemReplacementOptions = []
) throws -> NSURL?
```

