

- Foundation
- NSURL
-  promisedItemResourceValues(forKeys:) 

Instance Method

# promisedItemResourceValues(forKeys:)

Returns the resource values for the properties identified by specified array of keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func promisedItemResourceValues(forKeys keys: [URLResourceKey]) throws -> [URLResourceKey : Any]
```

## Parameters 

`keys`  

An array of names of URL resource properties.

## Return Value

A dictionary of resource values indexed by key.

## Discussion

This method behaves identically to resourceValues(forKeys:), but works on promised items. A promised item is not guaranteed to have its contents in the file system until you use a file coordinator to perform a coordinated read on its URL, which causes the contents to be downloaded or otherwise generated. Promised item URLs are returned by various APIs, including:

- A metadata query using either the NSMetadataQueryUbiquitousDataScope or NSMetadataQueryUbiquitousDocumentsScope scopes

- The contents of the directory returned by the file manager’s `URLForUbiquitousContainerIdentifier:`

- The URL inside the accessor block of a coordinated read or write operation that used the immediatelyAvailableMetadataOnly, forDeleting, forMoving, or contentIndependentMetadataOnly options

You must use this method instead of `resourceValuesForKeys:error:` for any URLs returned by these methods.

This method works for any resource value that is not tied to the item’s contents. Some keys, like contentAccessDateKey or generationIdentifierKey, do not return valid values. If you use one of these keys, the method returns true, but the value returns `nil`.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func resourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

### Working with Promised Items

func checkPromisedItemIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the promised item can be reached.

func getPromisedItemResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

