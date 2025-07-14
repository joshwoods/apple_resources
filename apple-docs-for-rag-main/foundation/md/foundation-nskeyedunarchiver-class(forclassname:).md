

- Foundation
- NSKeyedUnarchiver
-  class(forClassName:) 

Type Method

# class(forClassName:)

Returns the class from which this unarchiver instantiates an encoded object with a given class name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func `class`(forClassName codedName: String) -> AnyClass?
```

## Parameters 

`codedName`  

The ostensible name of a class in an archive.

## Return Value

The class from which `NSKeyedUnarchiver` instantiates an object encoded with the class name `codedName`. Returns `nil` if `NSKeyedUnarchiver` does not have a translation mapping for `codedName`.

## See Also

### Managing Class Names

class func setClass(AnyClass?, forClassName: String)

Sets a global translation mapping to decode objects encoded with a given class name as instances of a given class instead.

func setClass(AnyClass?, forClassName: String)

Sets a translation mapping on this unarchiver to decode objects encoded with a given class name as instances of a given class instead.

func `class`(forClassName: String) -> AnyClass?

Returns the class from which this unarchiver instantiates an encoded object with a given class name.

