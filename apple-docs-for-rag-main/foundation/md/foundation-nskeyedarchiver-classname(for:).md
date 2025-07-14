

- Foundation
- NSKeyedArchiver
-  className(for:) 

Type Method

# className(for:)

Returns the class name with which the archiver class encodes instances of a given class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func className(for cls: AnyClass) -> String?
```

## Parameters 

`cls`  

The class for which to determine the translation mapping.

## Return Value

The class name with which NSKeyedArchiver encodes instances of `cls`. Returns `nil` if NSKeyedArchiver does not have a translation mapping for `cls`.

## See Also

### Managing Classes and Class Names

class func setClassName(String?, for: AnyClass)

Sets a global translation mapping to encode instances of a given class with the provided name, rather than their real name.

func setClassName(String?, for: AnyClass)

Sets a mapping for this archiver to encode instances of a given class with the provided name, rather than their real name.

func className(for: AnyClass) -> String?

Returns the class name with which this archiver encodes instances of a given class.

