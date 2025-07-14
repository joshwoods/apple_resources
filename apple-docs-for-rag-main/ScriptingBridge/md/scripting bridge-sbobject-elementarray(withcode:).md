

- Scripting Bridge
- SBObject
-  elementArray(withCode:) 

Instance Method

# elementArray(withCode:)

Returns an array containing every child of the receiver with the given class-type code.

Mac Catalyst 13.0+macOS 10.5+

``` source
func elementArray(withCode code: DescType) -> SBElementArray
```

## Parameters 

`code`  

A four-character code that identifies a scripting class.

## Return Value

An SBElementArray object containing every child of the receiver whose class matches `code`.

## Discussion

`SBObject` subclasses use this method to implement application-specific property accessor methods. You should not need to call this method directly.

Note

This method doesn’t retrieve the value of the property. To get the value, call get().

## See Also

### Getting Properties and Elements

func property(with: AnyClass, code: AEKeyword) -> SBObject

Returns an object of the designated scripting class representing the specified property of the receiver

func property(withCode: AEKeyword) -> SBObject

Returns an object representing the specified property of the receiver.

