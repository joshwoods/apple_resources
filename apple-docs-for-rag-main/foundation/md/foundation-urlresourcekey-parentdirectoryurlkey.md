

- Foundation
- URLResourceKey
-  parentDirectoryURLKey 

Type Property

# parentDirectoryURLKey

The container directory of the resource.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let parentDirectoryURLKey: URLResourceKey
```

## Discussion

The corresponding value is a read-only `NSURL` object, or `nil` if the resource is the root directory of its volume.

## See Also

### Directory keys

static let isDirectoryKey: URLResourceKey

A key for determining whether the resource is a directory.

static let directoryEntryCountKey: URLResourceKey

The key for a count of items in the directory.

