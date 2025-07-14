

- CKTool JS
-  CKDBRecordFieldStringValue 

Structure

# CKDBRecordFieldStringValue

The value of the field of type string.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldStringValue {
 string type;
 string? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldStringValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

A string value.

## See Also

### Strings

CKDBRecordFieldStringListValue

The value of the field of type string list.

CKDBRecordFieldEncryptedStringValue

The value of the encrypted field of type string.

CKDBRecordFieldEncryptedStringListValue

The value of the encrypted field of type string list.

