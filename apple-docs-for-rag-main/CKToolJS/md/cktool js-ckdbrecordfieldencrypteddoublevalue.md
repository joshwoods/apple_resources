

- CKTool JS
-  CKDBRecordFieldEncryptedDoubleValue 

Structure

# CKDBRecordFieldEncryptedDoubleValue

The value of the encrypted field of type double.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldEncryptedDoubleValue {
 string type;
 Double? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldEncryptedDoubleValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

A double value.

## See Also

### Doubles

CKDBRecordFieldDoubleValue

The value of the field of type double.

CKDBRecordFieldDoubleListValue

The value of the field of type double list.

CKDBRecordFieldEncryptedDoubleListValue

The value of the encrypted field of type double list.

