

- Foundation
- NSKeyedUnarchiver
-  setClass(\_:forClassName:) 

Type Method

# setClass(\_:forClassName:)

Sets a global translation mapping to decode objects encoded with a given class name as instances of a given class instead.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func setClass(
    _ cls: AnyClass?,
    forClassName codedName: String
)
```

## Parameters 

`cls`  

The class with which to replace instances of the class named `codedName`.

`codedName`  

The ostensible name of a class in an archive.

## Discussion

When decoding, the class’s translation mapping is used only if no translation is found first in an instance’s separate translation map.

## See Also

### Managing Class Names

class func `class`(forClassName: String) -> AnyClass?

Returns the class from which this unarchiver instantiates an encoded object with a given class name.

func setClass(AnyClass?, forClassName: String)

Sets a translation mapping on this unarchiver to decode objects encoded with a given class name as instances of a given class instead.

func `class`(forClassName: String) -> AnyClass?

Returns the class from which this unarchiver instantiates an encoded object with a given class name.

