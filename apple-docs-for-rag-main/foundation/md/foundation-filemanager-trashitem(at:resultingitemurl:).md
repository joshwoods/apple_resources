

- Foundation
- FileManager
-  trashItem(at:resultingItemURL:) 

Instance Method

# trashItem(at:resultingItemURL:)

Moves an item to the trash.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+

``` source
func trashItem(
    at url: URL,
    resultingItemURL outResultingURL: AutoreleasingUnsafeMutablePointer?
) throws
```

## Parameters 

`url`  

The item to move to the trash.

`outResultingURL`  

On input, a pointer to a URL object. On output, this pointer is set to the item’s location in the trash. The actual name of the item may be changed when moving it to the trash, so use this URL to access it. You may specify `nil` for this parameter if you do not want the information.

## See Also

### Creating and Deleting Items

func createDirectory(at: URL, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with the given attributes at the specified URL.

func createDirectory(atPath: String, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with given attributes at the specified path.

func createFile(atPath: String, contents: Data?, attributes: [FileAttributeKey : Any]?) -> Bool

Creates a file with the specified content and attributes at the given location.

func removeItem(at: URL) throws

Removes the file or directory at the specified URL.

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

