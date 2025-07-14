

- AppKit
- NSCell
-  takeDoubleValueFrom(\_:) 

Instance Method

# takeDoubleValueFrom(\_:)

Sets the value of the receiver’s cell to a double-precision floating-point value obtained from the specified object.

macOS

``` source
@MainActor
func takeDoubleValueFrom(_ sender: Any?)
```

## Parameters 

`sender`  

The object from which to take the value. This object must implement the doubleValue property.

## See Also

### Related Documentation

var doubleValue: Double

The cell’s value as a double-precision floating-point number.

### Deriving Values

func takeObjectValueFrom(Any?)

Sets the value of the receiver’s cell to the object value obtained from the specified object.

func takeIntegerValueFrom(Any?)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

func takeIntValueFrom(Any?)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

func takeStringValueFrom(Any?)

Sets the value of the receiver’s cell to the string value obtained from the specified object.

func takeFloatValueFrom(Any?)

Sets the value of the receiver’s cell to a single-precision floating-point value obtained from the specified object.

