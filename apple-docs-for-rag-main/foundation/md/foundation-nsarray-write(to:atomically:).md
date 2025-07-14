

- Foundation
- NSArray
-  write(to:atomically:) 

Instance Method

# write(to:atomically:)

Writes the contents of the array to the location specified by a given URL.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func write(
    to url: URL,
    atomically: Bool
) -> Bool
```

## Parameters 

`url`  

The location at which to write the array.

`atomically`  

If true, the array is written to an auxiliary location, and then the auxiliary location is renamed to `aURL`. If false, the array is written directly to `aURL`. The true option guarantees that `aURL`, if it exists at all, won’t be corrupted even if the system should crash during writing.

## Return Value

true if the location is written successfully, otherwise false.

## Discussion

If the array’s contents are all property list objects (`NSString`, `NSData`, `NSArray`, or `NSDictionary` objects), the location written by this method can be used to initialize a new array with the class method init(contentsOfURL:) or the instance method init(contentsOfURL:).

## See Also

### Related Documentation

convenience init?(contentsOfURL: URL)

Initializes a newly allocated array with the contents of the location specified by a given URL.

### Storing Arrays

func write(toFile: String, atomically: Bool) -> Bool

Writes the contents of the array to a file at a given path.

