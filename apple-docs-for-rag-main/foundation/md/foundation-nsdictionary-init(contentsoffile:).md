

- Foundation
- NSDictionary
-  init(contentsOfFile:) 

Initializer

# init(contentsOfFile:)

Initializes a newly allocated dictionary using the keys and values found in a file at a given path.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
convenience init?(contentsOfFile path: String)
```

## Parameters 

`path`  

A full or relative pathname. The file identified by `path` must contain a string representation of a property list whose root object is a dictionary.

## Return Value

An initialized dictionary—which might be different than the original receiver—that contains the dictionary at `path`, or `nil` if there is a file error or if the contents of the file are an invalid representation of a dictionary.

## Discussion

The dictionary representation in the file identified by `path` must contain only property list objects (`NSString`, `NSData`, `NSDate`, `NSNumber`, `NSArray`, or `NSDictionary` objects). For more details, see Property List Programming Guide. The objects contained by this dictionary are immutable, even if the dictionary is mutable.

## See Also

### Creating a Dictionary from an External Source

init?(contentsOfURL: URL)

Creates a dictionary using the keys and values found in a resource specified by a given URL.

Deprecated

convenience init(contentsOfURL: URL, error: ()) throws

Initializes a newly allocated dictionary using the keys and values found at a given URL.

convenience init?(contentsOfURL: URL)

Initializes a newly allocated dictionary using the keys and values found at a given URL.

Deprecated

