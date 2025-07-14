

- AppKit
- NSCell
-  takeIntegerValueFrom(\_:) 

Instance Method

# takeIntegerValueFrom(\_:)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

macOS 10.5+

``` source
@MainActor
func takeIntegerValueFrom(_ sender: Any?)
```

## Parameters 

`sender`  

The object from which to take the value. This object must implement the integerValue property.

## See Also

### Related Documentation

var integerValue: Int

The cell’s value as an NSInteger type.

### Deriving Values

func takeObjectValueFrom(Any?)

Sets the value of the receiver’s cell to the object value obtained from the specified object.

func takeIntValueFrom(Any?)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

func takeStringValueFrom(Any?)

Sets the value of the receiver’s cell to the string value obtained from the specified object.

func takeDoubleValueFrom(Any?)

Sets the value of the receiver’s cell to a double-precision floating-point value obtained from the specified object.

func takeFloatValueFrom(Any?)

Sets the value of the receiver’s cell to a single-precision floating-point value obtained from the specified object.

