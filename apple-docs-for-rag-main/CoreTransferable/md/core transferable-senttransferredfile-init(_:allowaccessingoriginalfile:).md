

- Core Transferable
- SentTransferredFile
-  init(\_:allowAccessingOriginalFile:) 

Initializer

# init(\_:allowAccessingOriginalFile:)

Creates a description of a file from the perspective of the sender.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ file: URL,
    allowAccessingOriginalFile: Bool = false
)
```

## Parameters 

`file`  

A URL that describes the location of the file.

`allowAccessingOriginalFile`  

A Boolean value that indicates whether the receiver can read and write the original file. When set to `false`, the receiver can only gain access to a copy of the file.

## See Also

### Configuring a file transfer

let file: URL

A URL that describes the location of the file.

let allowAccessingOriginalFile: Bool

A Boolean value that indicates whether the receiver can read and write the original file. When set to `false`, the receiver can only gain access to a copy of the file.

