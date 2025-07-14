

- Foundation
- NSDictionary
-  write(to:) 

Instance Method

# write(to:)

Writes a property list representation of the contents of the dictionary to a given URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func write(to url: URL) throws
```

## Parameters 

`url`  

The URL to which to write the dictionary.

## Discussion

This method recursively validates that all the contained objects are property list objects (instances of NSData, NSDate, NSNumber, NSString, NSArray, or NSDictionary) before writing out the file. The method throws an error if all the objects are not property list objects, because the resulting output wouldn’t be a valid property list.

If the dictionary’s contents are all property list objects, you can use the location written by this method to initialize a new dictionary with the instance method init(contentsOfURL:).

If you need greater control over the property list representation, use PropertyListSerialization instead.

For more information about property lists, see Property List Programming Guide.

## See Also

### Storing Dictionaries

func write(to: URL, atomically: Bool) -> Bool

Writes a property list representation of the contents of the dictionary to a given URL.

Deprecated

func write(toFile: String, atomically: Bool) -> Bool

Writes a property list representation of the contents of the dictionary to a given path.

Deprecated

