

- CKTool JS
-  LengthError 

Class

# LengthError

The base class of length-related validation errors.

CKTool JS 1.2.15+

``` source
interface LengthError
```

## Overview

Extends `ValidationError`.

## Topics

### Instance Properties

value

The length value that failed validation.

## Relationships

### Inherits From

- LengthGreaterThanMaxError
- LengthLessThanMinError

### Inherited By

- ValidationError

## See Also

### Length Errors

LengthGreaterThanMaxError

An error a validator emits when the length property of the value given is greater than the allowed maximum.

LengthLessThanMinError

An error a validator emits when the length property of the value given is less than the allowed minimum.

LengthNotNumericError

An error a validator emits when the length property of a value isn’t numeric.

