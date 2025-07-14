

- Foundation
- NSURL
-  checkPromisedItemIsReachableAndReturnError(\_:) 

Instance Method

# checkPromisedItemIsReachableAndReturnError(\_:)

Returns whether the promised item can be reached.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func checkPromisedItemIsReachableAndReturnError(_ error: NSErrorPointer) -> Bool
```

## Parameters 

`error`  

The error that occurred when the promised item could not be reached.

## Return Value

true if the promised item is reachable; otherwise, false.

## Discussion

This method behaves identically to checkResourceIsReachableAndReturnError(_:), but works on promised items. A promised item is not guaranteed to have its contents in the file system until you use a file coordinator to perform a coordinated read on its URL, which causes the contents to be downloaded or otherwise generated. Promised item URLs are returned by various APIs, including:

- A metadata query using either the NSMetadataQueryUbiquitousDataScope or NSMetadataQueryUbiquitousDocumentsScope scopes

- The contents of the directory returned by the file manager’s `URLForUbiquitousContainerIdentifier:`

- The URL inside the accessor block of a coordinated read or write operation that used the immediatelyAvailableMetadataOnly, forDeleting, forMoving, or contentIndependentMetadataOnly options

You must use this method instead of `checkResourceIsReachableAndReturnError` for any URLs returned by these methods.

## See Also

### Related Documentation

func checkResourceIsReachableAndReturnError(NSErrorPointer) -> Bool

Returns whether the resource pointed to by a file URL can be reached.

### Working with Promised Items

func getPromisedItemResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

func promisedItemResourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

