

- CKTool JS
- CKToolDatabaseModule
-  toInt32 

Type Method

# toInt32

Converts a number to an `Int32`.

CKTool JS 1.2.15+

``` source
static Int32 toInt32();
```

## Parameters 

`value`  

A number to convert or validate.

## Return Value

If the value passes validation, this function returns an `Int32`; otherwise it throws `ValueNotInt32Error`. A numeric value passes validation if it’s within signed 32-bit integer range.

## Discussion

In TypeScript, `Int32` is a branded number type. In JavaScript, it’s a number.

```
import { toInt32 } from "@apple/cktool.database";
```

