

- Core Transferable
- SentTransferredFile
-  file 

Instance Property

# file

A URL that describes the location of the file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let file: URL
```

## See Also

### Configuring a file transfer

init(URL, allowAccessingOriginalFile: Bool)

Creates a description of a file from the perspective of the sender.

let allowAccessingOriginalFile: Bool

A Boolean value that indicates whether the receiver can read and write the original file. When set to `false`, the receiver can only gain access to a copy of the file.

