

- CKTool JS
- CKToolDatabaseModule
-  toInt64 

Type Method

# toInt64

Converts a number or numeric string to a `Int64`.

CKTool JS 1.2.15+

``` source
static Int64 toInt64();
```

## Parameters 

`value`  

A numeric or numeric string to convert or validate.

## Return Value

If the value passes validation, this function returns a `Int64`; otherwise it throws `ValueNotInt64Error`. A numeric value passes validation if it’s within signed 64-bit integer range. `toInt64` can accept a numeric string that represents a number that requires more precision than can be achieved with a JavaScript number.

## Discussion

In TypeScript, `Int64` is a branded `BigNumber` type. In JavaScript, it’s a `BigNumber`. `BigNumber` is from the bignumber.js package.

```
import { toInt64 } from "@apple/cktool.database";
```

