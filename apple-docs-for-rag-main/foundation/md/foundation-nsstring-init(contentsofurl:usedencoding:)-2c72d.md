

- Foundation
- NSString
-  init(contentsOfURL:usedEncoding:) 

Initializer

# init(contentsOfURL:usedEncoding:)

Returns an `NSString` object initialized by reading data from a given URL and returns by reference the encoding used to interpret the data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    contentsOfURL url: URL,
    usedEncoding enc: UnsafeMutablePointer?
) throws
```

``` source
convenience init(
    contentsOf url: URL,
    usedEncoding enc: UnsafeMutablePointer?
) throws
```

## Parameters 

`url`  

The URL from which to read data.

`enc`  

Upon return, if `url` is read successfully, contains the encoding used to interpret the data. For possible values, see NSStringEncoding.

## Return Value

An `NSString` object initialized by reading data from `url`. If `url` can’t be opened or the encoding cannot be determined, returns `nil`. The returned initialized object might be different from the original receiver

## Discussion

To read data with an unknown encoding, pass `0` as the `enc` parameter as in:

```
    NSURL *textFileURL = …;
    NSStringEncoding encoding = 0;
    NSError *error = nil;
    NSString *string = [[NSString alloc] initWithContentsOfURL:textFileURL usedEncoding:&encoding error:&error];
```

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

convenience init(contentsOfURL: URL, usedEncoding: UnsafeMutablePointer&lt;UInt>?) throws

Returns a string created by reading data from a given URL and returns by reference the encoding used to interpret the data.

### Creating and Initializing a String from an URL

convenience init(contentsOfURL: URL, encoding: UInt) throws

Returns a string created by reading data from a given URL interpreted using a given encoding.

convenience init(contentsOfURL: URL, encoding: UInt) throws

Returns an `NSString` object initialized by reading data from a given URL interpreted using a given encoding.

convenience init(contentsOfURL: URL, usedEncoding: UnsafeMutablePointer&lt;UInt>?) throws

Returns a string created by reading data from a given URL and returns by reference the encoding used to interpret the data.

