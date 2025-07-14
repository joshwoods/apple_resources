

- CKTool JS
- CKToolDatabaseModule
-  toByteArray 

Type Method

# toByteArray

Converts a numeric array to a `ByteArray`.

CKTool JS 1.2.15+

``` source
static ByteArray toByteArray();
```

## Parameters 

`value`  

A numeric array to convert or validate.

## Return Value

If the value passes validation, this function returns a `ByteArray`; otherwise it throws `ValueNotByteArrayError`. A numeric array passes validation if every element of the array is an integer in the range 0 to 255, inclusive.

## Discussion

In TypeScript, `ByteArray` is a branded `Uint8Array` type. In JavaScript, it’s a `Uint8Array`.

```
import { toByteArray } from "@apple/cktool.database";
```

