

- Foundation
- NSDictionary
-  init(contentsOfURL:) Deprecated

Initializer

# init(contentsOfURL:)

Creates a dictionary using the keys and values found in a resource specified by a given URL.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
init?(contentsOfURL url: URL)
```

Deprecated

Use dictionaryWithContentsOfURL:error: instead.

## Parameters 

`url`  

An URL that identifies a resource containing a string representation of a property list whose root object is a dictionary.

## Return Value

A new dictionary that contains the dictionary at `aURL`, or `nil` if there is an error or if the contents of the resource are an invalid representation of a dictionary.

## Discussion

The dictionary representation in the file identified by `aURL` must contain only property list objects (`NSString`, `NSData`, `NSDate`, `NSNumber`, `NSArray`, or `NSDictionary` objects). For more details, see Property List Programming Guide. The objects contained by this dictionary are immutable, even if the dictionary is mutable.

## See Also

### Creating a Dictionary from an External Source

convenience init(contentsOfURL: URL, error: ()) throws

Initializes a newly allocated dictionary using the keys and values found at a given URL.

convenience init?(contentsOfURL: URL)

Initializes a newly allocated dictionary using the keys and values found at a given URL.

Deprecated

convenience init?(contentsOfFile: String)

Initializes a newly allocated dictionary using the keys and values found in a file at a given path.

