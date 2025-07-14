

- CKTool JS
-  ValueLessThanMinNumberError 

Class

# ValueLessThanMinNumberError

An error a validator emits when a given value is less than the allowed minimum.

CKTool JS 1.2.15+

``` source
interface ValueLessThanMinNumberError
```

## Overview

Extends `ValueRangeError`.

## Topics

### Instance Properties

minimum

The minimum value (inclusive) for the tested length property.

## Relationships

### Inherited By

- ValueRangeError

## See Also

### Value Range Errors

ValueRangeError

The base class of range-related validation errors.

ValueGreaterThanMaxNumberError

An error a validator emits when a given value is greater than the allowed maximum.

ValueNotInNumberRangeError

An error a validator emits when a value can’t be represented by a JavaScript number due to being outside of the representable range.

