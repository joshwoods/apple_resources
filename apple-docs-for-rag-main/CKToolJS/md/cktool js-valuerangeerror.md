

- CKTool JS
-  ValueRangeError 

Class

# ValueRangeError

The base class of range-related validation errors.

CKTool JS 1.2.15+

``` source
interface ValueRangeError
```

## Overview

Extends `ValidationError`.

## Topics

### Instance Properties

value

The value that failed validation.

## Relationships

### Inherits From

- ValueGreaterThanMaxNumberError
- ValueLessThanMinNumberError
- ValueNotInNumberRangeError

### Inherited By

- ValidationError

## See Also

### Value Range Errors

ValueGreaterThanMaxNumberError

An error a validator emits when a given value is greater than the allowed maximum.

ValueLessThanMinNumberError

An error a validator emits when a given value is less than the allowed minimum.

ValueNotInNumberRangeError

An error a validator emits when a value can’t be represented by a JavaScript number due to being outside of the representable range.

