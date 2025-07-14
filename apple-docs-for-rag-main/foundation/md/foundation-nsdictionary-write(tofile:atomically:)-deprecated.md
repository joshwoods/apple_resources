

- Foundation
- NSDictionary
-  write(toFile:atomically:) Deprecated

Instance Method

# write(toFile:atomically:)

Writes a property list representation of the contents of the dictionary to a given path.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func write(
    toFile path: String,
    atomically useAuxiliaryFile: Bool
) -> Bool
```

Deprecated

Use write(to:) instead.

## Parameters 

`path`  

The path at which to write the file.

If `path` contains a tilde (~) character, you must expand it with expandingTildeInPath before invoking this method.

`useAuxiliaryFile`  

A flag that specifies whether the file should be written atomically.

If `useAuxiliaryFile` is true, the dictionary is written to an auxiliary file, and then the auxiliary file is renamed to `path`. If `useAuxiliaryFile` is false, the dictionary is written directly to `path`. The true option guarantees that `path`, if it exists at all, won’t be corrupted even if the system should crash during writing.

## Return Value

true if the file is written successfully, otherwise false.

## Discussion

This method recursively validates that all the contained objects are property list objects (instances of `NSData`, `NSDate`, `NSNumber`, `NSString`, `NSArray`, or `NSDictionary`) before writing out the file, and returns false if all the objects are not property list objects, since the resultant file would not be a valid property list.

If the dictionary’s contents are all property list objects, the file written by this method can be used to initialize a new dictionary with the class method dictionaryWithContentsOfFile: or the instance method init(contentsOfFile:).

If you need greater control over the property list representation, use PropertyListSerialization instead.

For more information about property lists, see Property List Programming Guide.

## See Also

### Storing Dictionaries

func write(to: URL) throws

Writes a property list representation of the contents of the dictionary to a given URL.

func write(to: URL, atomically: Bool) -> Bool

Writes a property list representation of the contents of the dictionary to a given URL.

Deprecated

