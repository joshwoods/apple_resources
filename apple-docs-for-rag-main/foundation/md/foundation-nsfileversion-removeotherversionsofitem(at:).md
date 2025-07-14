

- Foundation
- NSFileVersion
-  removeOtherVersionsOfItem(at:) 

Type Method

# removeOtherVersionsOfItem(at:)

Removes all versions of a file, except the current one, from the version store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func removeOtherVersionsOfItem(at url: URL) throws
```

## Parameters 

`url`  

The file whose older versions you want to delete. If the file at this URL does not exist, a new file is created at the location.

## Discussion

This method removes all versions except the current one from the version store, freeing up the associated storage space.

You should always remove file versions as part of a coordinated write operation to a file. In other words, always call this method from a block passed to a file coordinator object to initiate a write operation. Doing so ensures that no other processes are operating on the file while you remove the version information.

If successful, subsequent requests for the versions of the file reflect that only the current version is available. You can use this method to free up disk space by removing versions that are no longer needed.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Replacing and Deleting Versions

func replaceItem(at: URL, options: NSFileVersion.ReplacingOptions) throws -> URL

Replace the contents of the specified file with the contents of the current version’s file.

func remove() throws

Remove this version object and its associated file from the version store.

