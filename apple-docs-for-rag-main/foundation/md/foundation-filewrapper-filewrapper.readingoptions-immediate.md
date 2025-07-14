

- Foundation
- FileWrapper
- FileWrapper.ReadingOptions
-  immediate 

Type Property

# immediate

The option to read files immediately after creating a file wrapper.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var immediate: FileWrapper.ReadingOptions { get }
```

## Discussion

When you create a file wrapper and pass the immediate reading option, the content of the file is read immediately. Otherwise, file content is read only when requested, such as by accessing the regularFileContents, fileWrappers, serializedRepresentation, or symbolicLinkDestinationURL properties.

Reading a file immediately rather than lazily can help mitigate against reading errors caused by the user moving or deleting the file after a file wrapper is created. However, passing this option can result in unnecessary disk or network access—particularly when opening a document file package, which causes all of its directory contents to be enumerated and read preemptively.

Even when immediate is specified, FileWrapper may not read the contents of some file packages immediately. For example, because the contents of bundles are immutable to the user, FileWrapper may read the children of such a directory lazily as a performance optimization.

You can use this option to take a snapshot of a file or folder for writing later. For example, an application like TextEdit can use this option when creating new file wrappers to represent attachments that the user creates by copying and pasting or dragging and dropping from the Finder to a TextEdit document.

## See Also

### Constants

static var withoutMapping: FileWrapper.ReadingOptions

Whether file mapping for regular file wrappers is disallowed.

static var withoutMapping: FileWrapper.ReadingOptions

Whether file mapping for regular file wrappers is disallowed.

