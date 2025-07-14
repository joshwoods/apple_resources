

- AppKit
- NSCell
-  takeFloatValueFrom(\_:) 

Instance Method

# takeFloatValueFrom(\_:)

Sets the value of the receiver’s cell to a single-precision floating-point value obtained from the specified object.

macOS

``` source
@MainActor
func takeFloatValueFrom(_ sender: Any?)
```

## Parameters 

`sender`  

The object from which to take the value. This object must implement the floatValue property.

## See Also

### Related Documentation

var floatValue: Float

The cell’s value as a single-precision floating-point number.

### Deriving Values

func takeObjectValueFrom(Any?)

Sets the value of the receiver’s cell to the object value obtained from the specified object.

func takeIntegerValueFrom(Any?)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

func takeIntValueFrom(Any?)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

func takeStringValueFrom(Any?)

Sets the value of the receiver’s cell to the string value obtained from the specified object.

func takeDoubleValueFrom(Any?)

Sets the value of the receiver’s cell to a double-precision floating-point value obtained from the specified object.

