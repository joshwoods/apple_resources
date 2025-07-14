

- Foundation
- NSDictionary
-  init(contentsOfURL:error:) 

Initializer

# init(contentsOfURL:error:)

Initializes a newly allocated dictionary using the keys and values found at a given URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init(
    contentsOfURL url: URL,
    error: ()
) throws
```

``` source
convenience init(
    contentsOf url: URL,
    error: ()
) throws
```

## Parameters 

`url`  

A URL that identifies a resource containing a string representation of a property list whose root object is a dictionary.

`error`  

On failure, a reference to the error that occurred.

## Return Value

An initialized dictionary that contains the dictionary at `url`, or `nil` if there is an error or if the contents of the resource are an invalid representation of a dictionary.

## Discussion

The dictionary representation in the file identified by `url` must contain only property list objects (NSString, NSData, NSDate, NSNumber, NSArray, or NSDictionary objects). For more details, see Property List Programming Guide. The objects contained by this dictionary are immutable, even if the dictionary is mutable.

In Swift, this initializer throws if there is an error loading the URL, or if the contents of the resource are an invalid representation of a dictionary.

## See Also

### Creating a Dictionary from an External Source

init?(contentsOfURL: URL)

Creates a dictionary using the keys and values found in a resource specified by a given URL.

Deprecated

convenience init?(contentsOfURL: URL)

Initializes a newly allocated dictionary using the keys and values found at a given URL.

Deprecated

convenience init?(contentsOfFile: String)

Initializes a newly allocated dictionary using the keys and values found in a file at a given path.

