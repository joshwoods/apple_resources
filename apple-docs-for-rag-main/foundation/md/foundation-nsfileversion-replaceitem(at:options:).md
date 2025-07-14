

- Foundation
- NSFileVersion
-  replaceItem(at:options:) 

Instance Method

# replaceItem(at:options:)

Replace the contents of the specified file with the contents of the current version’s file.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceItem(
    at url: URL,
    options: NSFileVersion.ReplacingOptions = []
) throws -> URL
```

## Parameters 

`url`  

The file whose contents you want to replace. If the file at this URL does not exist, a new file is created at the location.

`options`  

Specify `0` to overwrite the file in place; otherwise, specify one of the constants described in NSFileVersion.ReplacingOptions.

## Return Value

The URL of the file that was written, which may be different than the one specified in the `url` parameter.

## Discussion

When replacing the contents of the file, this method does not normally replace the display name associated with the file. The only exception is when the file at `url` is of a different type than the file associated with this version object. In such a case, the file name remains the same but its filename extension changes to match the type of the new contents. (Of course, if filename extension hiding is enabled, this change is not noticeable to users.)

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Replacing and Deleting Versions

func remove() throws

Remove this version object and its associated file from the version store.

class func removeOtherVersionsOfItem(at: URL) throws

Removes all versions of a file, except the current one, from the version store.

