

- Foundation
- NSURL
-  resourceValues(forKeys:) 

Instance Method

# resourceValues(forKeys:)

Returns the resource values for the properties identified by specified array of keys.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func resourceValues(forKeys keys: [URLResourceKey]) throws -> [URLResourceKey : Any]
```

## Parameters 

`keys`  

An array of property keys for the desired resource properties.

## Return Value

A dictionary of resource values indexed by key.

## Discussion

This method first checks if the URL object already caches the specified resource values. If so, it returns the cached resource values to the caller. If not, then this method synchronously obtains the resource values from the backing store, adds the resource values to the URL object’s cache, and returns the resource values to the caller.

The type of the returned resource value varies by resource property; for details, see the documentation for the key you want to access.

If the result dictionary does not contain a resource value for one or more of the requested resource keys, it means those resource properties are not available for the URL, and no errors occurred when determining those resource properties were not available.

If an error occurs, this method returns `nil` and populates the object pointer referenced by `error` with additional information.

Note

This method applies only to URLs that represent file system resources.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Accessing Resource Values

func getResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

func setResourceValue(Any?, forKey: URLResourceKey) throws

Sets the URL’s resource property for a given key to a given value.

func setResourceValues([URLResourceKey : Any]) throws

Sets the URL’s resource properties for a given set of keys to a given set of values.

func removeAllCachedResourceValues()

Removes all cached resource values and temporary resource values from the URL object.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given key from the URL object.

func setTemporaryResourceValue((any Sendable)?, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

