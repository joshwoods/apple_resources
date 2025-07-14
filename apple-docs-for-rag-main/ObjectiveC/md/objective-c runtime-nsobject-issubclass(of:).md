

- Objective-C Runtime
- NSObject
-  isSubclass(of:) 

Type Method

# isSubclass(of:)

Returns a Boolean value that indicates whether the receiving class is a subclass of, or identical to, a given class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func isSubclass(of aClass: AnyClass) -> Bool
```

## Parameters 

`aClass`  

A class object.

## Return Value

YES if the receiving class is a subclass of—or identical to—`aClass`, otherwise NO.

## See Also

### Identifying Classes

class func superclass() -> AnyClass?

Returns the class object for the receiver’s superclass.

