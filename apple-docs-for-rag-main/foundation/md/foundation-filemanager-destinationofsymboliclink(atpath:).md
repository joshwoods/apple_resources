

- Foundation
- FileManager
-  destinationOfSymbolicLink(atPath:) 

Instance Method

# destinationOfSymbolicLink(atPath:)

Returns the path of the item pointed to by a symbolic link.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func destinationOfSymbolicLink(atPath path: String) throws -> String
```

## Parameters 

`path`  

The path of a file or directory.

## Return Value

An NSString object containing the path of the directory or file to which the symbolic link `path` refers. When using Objective-C, returns `nil` upon failure. If the symbolic link is specified as a relative path, that relative path is returned.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating Symbolic and Hard Links

func createSymbolicLink(at: URL, withDestinationURL: URL) throws

Creates a symbolic link at the specified URL that points to an item at the given URL.

func createSymbolicLink(atPath: String, withDestinationPath: String) throws

Creates a symbolic link that points to the specified destination.

func linkItem(at: URL, to: URL) throws

Creates a hard link between the items at the specified URLs.

func linkItem(atPath: String, toPath: String) throws

Creates a hard link between the items at the specified paths.

