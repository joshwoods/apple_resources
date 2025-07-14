

- CKTool JS
-  CKDBRecordFieldInt64ListValue 

Structure

# CKDBRecordFieldInt64ListValue

The value of the field of type int64 list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldInt64ListValue {
 string type;
 Int64[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldInt64ListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An array of int64 values.

## See Also

### Int64

CKDBRecordFieldInt64Value

The value of the field of type int64.

CKDBRecordFieldEncryptedInt64Value

The value of the encrypted field of type int64.

CKDBRecordFieldEncryptedInt64ListValue

The value of the encrypted field of type int64 list.

