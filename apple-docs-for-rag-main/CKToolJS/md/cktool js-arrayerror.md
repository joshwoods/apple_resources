

- CKTool JS
-  ArrayError 

Class

# ArrayError

An error an array validator emits when an array’s elements fail validation.

CKTool JS 1.2.15+

``` source
interface ArrayError
```

## Overview

Extends `ValidationError`. The indices of the elements that failed validation are in the `indices` member. The `errors` array has the errors that correspond to the elements identified by the `indices` member.

## Topics

### Instance Properties

array

The array that failed validation.

errors

An array of errors that correspond to indexes.

indices

An array of indexes of elements that failed validation in the array.

## Relationships

### Inherited By

- ValidationError

## See Also

### Validation Errors

ValidationError

The base class of errors emitted when validators fail validation.

MaxValueNotNumericError

An error a validator emits when the maximum value given isn’t numeric.

MinValueNotNumericError

An error a validator emits when the minimum value given isn’t numeric.

ValueIsRequiredError

The error emitted when a value is required but a validator determines the value is not present.

ValueNotConvertibleToTypeError

The base class of errors related to type validation or coercion.

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

