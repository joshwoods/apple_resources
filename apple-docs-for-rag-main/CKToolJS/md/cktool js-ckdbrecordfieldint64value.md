

- CKTool JS
-  CKDBRecordFieldInt64Value 

Structure

# CKDBRecordFieldInt64Value

The value of the field of type int64.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldInt64Value {
 string type;
 Int64? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldInt64Value } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An int64 value.

## See Also

### Int64

CKDBRecordFieldInt64ListValue

The value of the field of type int64 list.

CKDBRecordFieldEncryptedInt64Value

The value of the encrypted field of type int64.

CKDBRecordFieldEncryptedInt64ListValue

The value of the encrypted field of type int64 list.

