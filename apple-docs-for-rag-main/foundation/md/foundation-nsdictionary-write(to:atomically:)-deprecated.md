

- Foundation
- NSDictionary
-  write(to:atomically:) Deprecated

Instance Method

# write(to:atomically:)

Writes a property list representation of the contents of the dictionary to a given URL.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func write(
    to url: URL,
    atomically: Bool
) -> Bool
```

Deprecated

Use write(to:) instead.

## Parameters 

`url`  

The URL to which to write the dictionary.

`atomically`  

A flag that specifies whether the output should be written atomically.

If `atomically` is true, the dictionary is written to an auxiliary location, and then the auxiliary location is renamed to `url`. If `atomically` is false, the dictionary is written directly to `url`. The true option guarantees that `url`, if it exists at all, won’t be corrupted even if the system should crash during writing. `atomically` is ignored if `url` is of a type that cannot be written atomically.

## Return Value

true if the location is written successfully, otherwise false.

## Discussion

This method recursively validates that all the contained objects are property list objects (instances of `NSData`, `NSDate`, `NSNumber`, `NSString`, `NSArray`, or `NSDictionary`) before writing out the file, and returns false if all the objects are not property list objects, since the resultant output would not be a valid property list.

If the dictionary’s contents are all property list objects, the location written by this method can be used to initialize a new dictionary with the class method init(contentsOfURL:) or the instance method init(contentsOfURL:).

If you need greater control over the property list representation, use PropertyListSerialization instead.

For more information about property lists, see Property List Programming Guide.

## See Also

### Storing Dictionaries

func write(to: URL) throws

Writes a property list representation of the contents of the dictionary to a given URL.

func write(toFile: String, atomically: Bool) -> Bool

Writes a property list representation of the contents of the dictionary to a given path.

Deprecated

