

- CKTool JS
- CKToolDatabaseModule
-  toBase64String 

Type Method

# toBase64String

Converts a regular string to a `Base64String`.

CKTool JS 1.2.15+

``` source
static Base64String toBase64String();
```

## Parameters 

`value`  

A string value to convert or validate.

## Return Value

If the value passes validation, this function returns a `Base64String`; otherwise it throws `ValueNotBase64StringError`. A string passes validation if it is a base 64 string.

## Discussion

In TypeScript, `Base64String` is a branded string type. In JavaScript, it’s a string.

```
import { toBase64String } from "@apple/cktool.database";
```

