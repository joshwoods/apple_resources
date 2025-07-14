

- Scripting Bridge
- SBObject
-  property(with:code:) 

Instance Method

# property(with:code:)

Returns an object of the designated scripting class representing the specified property of the receiver

Mac Catalyst 13.0+macOS 10.5+

``` source
func property(
    with cls: AnyClass,
    code: AEKeyword
) -> SBObject
```

## Parameters 

`code`  

A four-character code that uniquely identifies a property of the receiver.

## Return Value

An instance of the designated `class` that represents the receiver’s property identified by `code`.

## Discussion

`SBObject` subclasses use this method to implement application-specific property accessor methods. You should not need to call this method directly.

Note

This method doesn’t retrieve the value of the property. To get the value, call get().

## See Also

### Getting Properties and Elements

func property(withCode: AEKeyword) -> SBObject

Returns an object representing the specified property of the receiver.

func elementArray(withCode: DescType) -> SBElementArray

Returns an array containing every child of the receiver with the given class-type code.

