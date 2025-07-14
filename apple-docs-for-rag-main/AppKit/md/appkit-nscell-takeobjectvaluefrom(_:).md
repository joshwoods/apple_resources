

- AppKit
- NSCell
-  takeObjectValueFrom(\_:) 

Instance Method

# takeObjectValueFrom(\_:)

Sets the value of the receiver’s cell to the object value obtained from the specified object.

macOS

``` source
@MainActor
func takeObjectValueFrom(_ sender: Any?)
```

## Parameters 

`sender`  

The object from which to take the value. This object must support the objectValue property.

## See Also

### Related Documentation

var objectValue: Any?

The cell’s value as an Objective-C object.

### Deriving Values

func takeIntegerValueFrom(Any?)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

func takeIntValueFrom(Any?)

Sets the value of the receiver’s cell to an integer value obtained from the specified object.

func takeStringValueFrom(Any?)

Sets the value of the receiver’s cell to the string value obtained from the specified object.

func takeDoubleValueFrom(Any?)

Sets the value of the receiver’s cell to a double-precision floating-point value obtained from the specified object.

func takeFloatValueFrom(Any?)

Sets the value of the receiver’s cell to a single-precision floating-point value obtained from the specified object.

