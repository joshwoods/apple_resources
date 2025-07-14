

- Foundation
- NSURL
-  setResourceValue(\_:forKey:) 

Instance Method

# setResourceValue(\_:forKey:)

Sets the URL’s resource property for a given key to a given value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setResourceValue(
    _ value: Any?,
    forKey key: URLResourceKey
) throws
```

## Parameters 

`value`  

The value for the resource property defined by `key`.

`key`  

The name of one of the URL’s resource properties.

## Discussion

This method synchronously writes the new resource value out to disk. Attempts to set a read-only resource property or to set a resource property that is not supported by the resource are ignored and are not considered errors.

If an error occurs, this method returns false and populates the object pointer referenced by `error` with additional information.

Note

This method applies only to URLs for file system resources.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Accessing Resource Values

func resourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

func getResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

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

