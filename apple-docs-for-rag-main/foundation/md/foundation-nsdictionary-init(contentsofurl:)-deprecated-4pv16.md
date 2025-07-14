

- Foundation
- NSDictionary
-  init(contentsOfURL:) Deprecated

Initializer

# init(contentsOfURL:)

Initializes a newly allocated dictionary using the keys and values found at a given URL.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
convenience init?(contentsOfURL url: URL)
```

``` source
convenience init?(contentsOf url: URL)
```

Deprecated

Use init(contentsOfURL:error:) instead.

## Parameters 

`url`  

An URL that identifies a resource containing a string representation of a property list whose root object is a dictionary.

## Return Value

An initialized dictionary—which might be different than the original receiver—that contains the dictionary at `url`, or `nil` if there is an error or if the contents of the resource are an invalid representation of a dictionary.

## Discussion

The dictionary representation in the file identified by `url` must contain only property list objects (`NSString`, `NSData`, `NSDate`, `NSNumber`, `NSArray`, or `NSDictionary` objects). For more details, see Property List Programming Guide. The objects contained by this dictionary are immutable, even if the dictionary is mutable.

## See Also

### Related Documentation

init?(contentsOfURL: URL)

Creates a dictionary using the keys and values found in a resource specified by a given URL.

Deprecated

### Creating a Dictionary from an External Source

init?(contentsOfURL: URL)

Creates a dictionary using the keys and values found in a resource specified by a given URL.

Deprecated

convenience init(contentsOfURL: URL, error: ()) throws

Initializes a newly allocated dictionary using the keys and values found at a given URL.

convenience init?(contentsOfFile: String)

Initializes a newly allocated dictionary using the keys and values found in a file at a given path.

