

- CKTool JS
- CKToolDatabaseModule
-  toUuid 

Type Method

# toUuid

Converts a string to a `Uuid`.

CKTool JS 1.2.15+

``` source
static Uuid toUuid();
```

## Parameters 

`value`  

A string to convert or validate.

## Return Value

If the value passes validation, this function returns a `Uuid`; otherwise it throws `ValueNotUuidError`. A string passes validation if it is a UUID string.

## Discussion

In TypeScript, `Uuid` is a branded string type. In JavaScript, it’s a string.

```
import { toUuid } from "@apple/cktool.database";
```

