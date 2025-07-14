

- CKTool JS
- CKToolDatabaseModule
-  toByte 

Type Method

# toByte

Converts a numeric value to a `Byte`.

CKTool JS 1.2.15+

``` source
static Byte toByte();
```

## Parameters 

`value`  

A numeric value to convert or validate.

## Return Value

If the value passes validation, this function returns a `Byte`; otherwise it throws `ValueNotByteError`. A numeric value passes validation if it’s an integer in the range 0 to 255, inclusive.

## Discussion

In TypeScript, `Byte` is a branded number type. In JavaScript, it’s a number.

```
import { toByte } from "@apple/cktool.database";
```

