

- Foundation
- NSString
-  init(contentsOfURL:encoding:) 

Initializer

# init(contentsOfURL:encoding:)

Returns a string created by reading data from a given URL interpreted using a given encoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    contentsOfURL url: URL,
    encoding enc: UInt
) throws
```

## Parameters 

`url`  

The URL to read.

`enc`  

The encoding of the data at `url`. For possible values, see NSStringEncoding.

## Return Value

A string created by reading data from `URL` using the encoding, `enc`. If the URL can’t be opened or there is an encoding error, returns `nil`.

## See Also

### Creating and Initializing a String from an URL

convenience init(contentsOfURL: URL, encoding: UInt) throws

Returns an `NSString` object initialized by reading data from a given URL interpreted using a given encoding.

convenience init(contentsOfURL: URL, usedEncoding: UnsafeMutablePointer&lt;UInt>?) throws

Returns a string created by reading data from a given URL and returns by reference the encoding used to interpret the data.

convenience init(contentsOfURL: URL, usedEncoding: UnsafeMutablePointer&lt;UInt>?) throws

Returns an `NSString` object initialized by reading data from a given URL and returns by reference the encoding used to interpret the data.

