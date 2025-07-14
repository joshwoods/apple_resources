

- CKTool JS
- CKToolDatabaseModule
-  toDouble 

Type Method

# toDouble

Converts a number or numeric string to a `Double`.

CKTool JS 1.2.15+

``` source
static Double toDouble();
```

## Parameters 

`value`  

A numeric or numeric string to convert or validate.

## Return Value

If the value passes validation, this function returns a `Double`; otherwise it throws `ValueNotDoubleError`. A value passes validation if it’s a number in the range of a double-precision 64-bit IEEE 754 floating-point value. `toDouble` can also accept a numeric string that represents a number that requires more precision than can be achieved with a JavaScript number.

## Discussion

In TypeScript, `Double` is a branded `BigNumber` type. In JavaScript, it’s a `BigNumber`. `BigNumber` is from the bignumber.js package.

```
import { toDouble } from "@apple/cktool.database";
```

