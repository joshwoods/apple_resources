

- CKTool JS
-  ValueNotConvertibleToTypeError 

Class

# ValueNotConvertibleToTypeError

The base class of errors related to type validation or coercion.

CKTool JS 1.2.15+

``` source
interface ValueNotConvertibleToTypeError
```

## Overview

Extends `ValidationError`.

## Topics

### Instance Properties

typeDescription

The name of the type that the value should have been.

value

The value that failed validation.

## Relationships

### Inherits From

- LengthNotNumericError
- ValueNotArrayBufferError
- ValueNotArrayError
- ValueNotBase64StringError
- ValueNotBlobError
- ValueNotBooleanError
- ValueNotByteArrayError
- ValueNotByteError
- ValueNotDateError
- ValueNotDateStringError
- ValueNotDoubleError
- ValueNotEnumValueError
- ValueNotFloatError
- ValueNotFunctionError
- ValueNotInt32Error
- ValueNotInt64Error
- ValueNotJsonError
- ValueNotNumericError
- ValueNotStringError
- ValueNotUuidError

### Inherited By

- ValidationError

## See Also

### Validation Errors

ValidationError

The base class of errors emitted when validators fail validation.

ArrayError

An error an array validator emits when an array’s elements fail validation.

MaxValueNotNumericError

An error a validator emits when the maximum value given isn’t numeric.

MinValueNotNumericError

An error a validator emits when the minimum value given isn’t numeric.

ValueIsRequiredError

The error emitted when a value is required but a validator determines the value is not present.

ValueNotFunctionError

An error a validator emits when a value isn’t a function.

ValueNotArrayBufferError

An error a validator emits when a value isn’t an `ArrayBuffer`.

ValueNotArrayError

An error a validator emits when a value isn’t an array.

ValueNotBase64StringError

An error a validator emits when a value isn’t a `Base64` string or isn’t castable to that type.

ValueNotBlobError

An error a validator emits when a value isn’t a `Blob`.

ValueNotBooleanError

An error a validator emits when a value isn’t a Boolean or isn’t castable to that type.

ValueNotByteArrayError

An error a validator emits when a value isn’t a `ByteArray` or isn’t castable to that type.

ValueNotByteError

An error a validator emits when a value isn’t a `Byte` or isn’t castable to that type.

ValueNotDateError

An error a validator emits when a value isn’t a `Date` or isn’t castable to that type.

ValueNotDateStringError

An error a validator emits when a value isn’t a date string.

