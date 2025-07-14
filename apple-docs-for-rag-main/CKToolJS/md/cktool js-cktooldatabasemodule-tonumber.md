

- CKTool JS
- CKToolDatabaseModule
-  toNumber 

Type Method

# toNumber

Converts a supported numeric type to a JavaScript number.

CKTool JS 1.2.15+

``` source
static number toNumber();
```

## Parameters 

`value`  

A numeric value to convert or validate.

## Discussion

If the value passed in isn’t a number, this function throws `ValueNotNumericError`. If the value is numeric but can’t be represented by a JavaScript number, it throws `ValueNotInNumberRangeError`.

```
import { toNumber } from "@apple/cktool.database";
```

