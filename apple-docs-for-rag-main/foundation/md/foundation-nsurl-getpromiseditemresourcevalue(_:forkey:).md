

- Foundation
- NSURL
-  getPromisedItemResourceValue(\_:forKey:) 

Instance Method

# getPromisedItemResourceValue(\_:forKey:)

Returns the value of the resource property for the specified key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getPromisedItemResourceValue(
    _ value: AutoreleasingUnsafeMutablePointer,
    forKey key: URLResourceKey
) throws
```

## Parameters 

`value`  

The location where the value for the resource property identified by `key` should be stored.

`key`  

The name of one of the URL’s resource properties.

## Discussion

This method behaves identically to getResourceValue(_:forKey:), but works on promised items. A promised item is not guaranteed to have its contents in the file system until you use a file coordinator to perform a coordinated read on its URL, which causes the contents to be downloaded or otherwise generated. Promised item URLs are returned by various APIs, including:

- A metadata query using either the NSMetadataQueryUbiquitousDataScope or NSMetadataQueryUbiquitousDocumentsScope scopes

- The contents of the directory returned by the file manager’s `URLForUbiquitousContainerIdentifier:`

- The URL inside the accessor block of a coordinated read or write operation that used the immediatelyAvailableMetadataOnly, forDeleting, forMoving, or contentIndependentMetadataOnly options

You must use this method instead of `getResourceValue:forKey:error:` for any URLs returned by these methods.

This method works for any resource value that is not tied to the item’s contents. Some keys, like contentAccessDateKey or generationIdentifierKey, do not return valid values. If you use one of these keys, the method returns true, but the value returns `nil`.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func getResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

### Working with Promised Items

func checkPromisedItemIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the promised item can be reached.

func promisedItemResourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

