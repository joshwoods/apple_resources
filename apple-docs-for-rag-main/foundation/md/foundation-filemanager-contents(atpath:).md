

- Foundation
- FileManager
-  contents(atPath:) 

Instance Method

# contents(atPath:)

Returns the contents of the file at the specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contents(atPath path: String) -> Data?
```

## Parameters 

`path`  

The path of the file whose contents you want.

## Return Value

An NSData object with the contents of the file. If `path` specifies a directory, or if some other error occurs, this method returns `nil`.

## See Also

### Related Documentation

func createFile(atPath: String, contents: Data?, attributes: [FileAttributeKey : Any]?) -> Bool

Creates a file with the specified content and attributes at the given location.

### Getting and Comparing File Contents

func contentsEqual(atPath: String, andPath: String) -> Bool

Returns a Boolean value that indicates whether the files or directories in specified paths have the same contents.

