

- CKTool JS
-  Database, Length, Validation, and Value Errors 

API Collection

# Database, Length, Validation, and Value Errors

## Topics

### Database Errors

AuthenticationRequiredError

An object that represents an error that occurs when authentication information is missing for the current user.

CKDBBatchDeleteError

An object that represents an error that may occur when deleting a resource as part of a batch delete operation.

RequestError

An object that represents a general error from the service.

### Length Errors

LengthError

The base class of length-related validation errors.

LengthGreaterThanMaxError

An error a validator emits when the length property of the value given is greater than the allowed maximum.

LengthLessThanMinError

An error a validator emits when the length property of the value given is less than the allowed minimum.

LengthNotNumericError

An error a validator emits when the length property of a value isn’t numeric.

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

ValueNotDoubleError

An error a validator emits when a value isn’t a `Double` or isn’t castable to that type.

ValueNotEnumValueError

An error a validator emits when a value isn’t a valid enumeration value.

ValueNotFloatError

An error a validator emits when a value isn’t a `Float` or isn’t castable to that type.

ValueNotInt32Error

An error a validator emits when a value isn’t an `Int32` or isn’t castable to that type.

ValueNotInt64Error

An error a validator emits when a value isn’t an `Int64` or isn’t castable to that type.

ValueNotJsonError

An error a validator emits when a value isn’t JSON.

ValueNotNumericError

An error a validator emits when a value isn’t numeric.

ValueNotObjectError

An error a validator emits when a value isn’t an object.

ValueNotStringError

An error a validator emits when a value isn’t a string.

ValueNotUuidError

An error a validator emits when a value isn’t a `Uuid` or isn’t castable to that type.

ValueTypeNotRecognizedError

An error that a deserializer emits when it fails to recognize the type of object to deserialize or process.

### Value Range Errors

ValueRangeError

The base class of range-related validation errors.

ValueGreaterThanMaxNumberError

An error a validator emits when a given value is greater than the allowed maximum.

ValueLessThanMinNumberError

An error a validator emits when a given value is less than the allowed minimum.

ValueNotInNumberRangeError

An error a validator emits when a value can’t be represented by a JavaScript number due to being outside of the representable range.

## See Also

### Errors

ErrorBase

The base class of any error emitted by functions in the client library.

