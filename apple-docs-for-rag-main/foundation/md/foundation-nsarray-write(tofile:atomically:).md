

- Foundation
- NSArray
-  write(toFile:atomically:) 

Instance Method

# write(toFile:atomically:)

Writes the contents of the array to a file at a given path.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func write(
    toFile path: String,
    atomically useAuxiliaryFile: Bool
) -> Bool
```

## Parameters 

`path`  

The path at which to write the contents of the array.

If `path` contains a tilde (~) character, you must expand it with expandingTildeInPath before invoking this method.

`useAuxiliaryFile`  

If true, the array is written to an auxiliary file, and then the auxiliary file is renamed to `path`. If false, the array is written directly to `path`. The true option guarantees that `path`, if it exists at all, won’t be corrupted even if the system should crash during writing.

## Return Value

true if the file is written successfully, otherwise false.

## Discussion

If the array’s contents are all property list objects (`NSString`, `NSData`, `NSArray`, or `NSDictionary` objects), the file written by this method can be used to initialize a new array with the class method arrayWithContentsOfFile: or the instance method init(contentsOfFile:). This method recursively validates that all the contained objects are property list objects before writing out the file, and returns false if all the objects are not property list objects, since the resultant file would not be a valid property list.

## See Also

### Related Documentation

convenience init?(contentsOfFile: String)

Initializes a newly allocated array with the contents of the file specified by a given path.

### Storing Arrays

func write(to: URL, atomically: Bool) -> Bool

Writes the contents of the array to the location specified by a given URL.

