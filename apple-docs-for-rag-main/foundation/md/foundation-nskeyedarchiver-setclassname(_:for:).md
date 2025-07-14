

- Foundation
- NSKeyedArchiver
-  setClassName(\_:for:) 

Type Method

# setClassName(\_:for:)

Sets a global translation mapping to encode instances of a given class with the provided name, rather than their real name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func setClassName(
    _ codedName: String?,
    for cls: AnyClass
)
```

## Parameters 

`codedName`  

The name of the class that `NSKeyedArchiver` uses in place of `cls`.

`cls`  

The class for which to set up a translation mapping.

## Discussion

When encoding, an archiver consults its own translation map before using the class’ translation map.

## See Also

### Managing Classes and Class Names

class func className(for: AnyClass) -> String?

Returns the class name with which the archiver class encodes instances of a given class.

func setClassName(String?, for: AnyClass)

Sets a mapping for this archiver to encode instances of a given class with the provided name, rather than their real name.

func className(for: AnyClass) -> String?

Returns the class name with which this archiver encodes instances of a given class.

