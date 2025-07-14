

- Scripting Bridge
- SBObject
-  property(withCode:) 

Instance Method

# property(withCode:)

Returns an object representing the specified property of the receiver.

Mac Catalyst 13.0+macOS 10.5+

``` source
func property(withCode code: AEKeyword) -> SBObject
```

## Parameters 

`code`  

A four-character code that uniquely identifies a property of the receiver.

## Return Value

An object representing the receiver’s property as identified by `code`.

## Discussion

`SBObject` subclasses use this method to implement application-specific property accessor methods. You should not need to call this method directly.

## See Also

### Getting Properties and Elements

func property(with: AnyClass, code: AEKeyword) -> SBObject

Returns an object of the designated scripting class representing the specified property of the receiver

func elementArray(withCode: DescType) -> SBElementArray

Returns an array containing every child of the receiver with the given class-type code.

