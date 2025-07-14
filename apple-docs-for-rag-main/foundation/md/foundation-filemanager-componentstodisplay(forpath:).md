

- Foundation
- FileManager
-  componentsToDisplay(forPath:) 

Instance Method

# componentsToDisplay(forPath:)

Returns an array of strings representing the user-visible components of a given path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func componentsToDisplay(forPath path: String) -> [String]?
```

## Parameters 

`path`  

A pathname.

## Return Value

An array of NSString objects representing the user-visible (for the Finder, Open and Save panels, and so on) components of `path`. Returns `nil` if path does not exist.

## Discussion

These components cannot be used for path operations and are only suitable for display to the user.

## See Also

### Getting and Setting Attributes

func displayName(atPath: String) -> String

Returns the display name of the file or directory at a specified path.

func attributesOfItem(atPath: String) throws -> [FileAttributeKey : Any]

Returns the attributes of the item at a given path.

func attributesOfFileSystem(forPath: String) throws -> [FileAttributeKey : Any]

Returns a dictionary that describes the attributes of the mounted file system on which a given path resides.

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

