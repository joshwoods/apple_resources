

- Foundation
- NSURL
-  isFileURL 

Instance Property

# isFileURL

A boolean value that determines whether the receiver is a file URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isFileURL: Bool { get }
```

## Discussion

The property’s value is true if the receiver uses the file scheme, false otherwise. Both file path and file reference URLs are considered to be file URLs.

If this property’s value is true, then the receiver’s path property contains a suitable value for input into FileManager or `NSPathUtilities`.

## See Also

### Querying an NSURL

func checkResourceIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

func isFileReferenceURL() -> Bool

Returns whether the URL is a file reference URL.

