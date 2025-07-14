

- Foundation
- NSString
-  init(contentsOfURL:encoding:) 

Initializer

# init(contentsOfURL:encoding:)

Returns an `NSString` object initialized by reading data from a given URL interpreted using a given encoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    contentsOfURL url: URL,
    encoding enc: UInt
) throws
```

``` source
convenience init(
    contentsOf url: URL,
    encoding enc: UInt
) throws
```

## Parameters 

`url`  

The URL to read.

`enc`  

The encoding of the file at `path`. For possible values, see NSStringEncoding.

## Return Value

An `NSString` object initialized by reading data from `url`. The returned object may be different from the original receiver. If the URL can’t be opened or there is an encoding error, returns `nil`.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

convenience init(contentsOfURL: URL, encoding: UInt) throws

Returns a string created by reading data from a given URL interpreted using a given encoding.

### Creating and Initializing a String from an URL

convenience init(contentsOfURL: URL, encoding: UInt) throws

Returns a string created by reading data from a given URL interpreted using a given encoding.

convenience init(contentsOfURL: URL, usedEncoding: UnsafeMutablePointer&lt;UInt>?) throws

Returns a string created by reading data from a given URL and returns by reference the encoding used to interpret the data.

convenience init(contentsOfURL: URL, usedEncoding: UnsafeMutablePointer&lt;UInt>?) throws

Returns an `NSString` object initialized by reading data from a given URL and returns by reference the encoding used to interpret the data.

