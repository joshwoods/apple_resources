

- CKTool JS
-  CKDBRecordFieldEncryptedDoubleListValue 

Structure

# CKDBRecordFieldEncryptedDoubleListValue

The value of the encrypted field of type double list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldEncryptedDoubleListValue {
 string type;
 Double[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldEncryptedDoubleListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An array of double values.

## See Also

### Doubles

CKDBRecordFieldDoubleValue

The value of the field of type double.

CKDBRecordFieldDoubleListValue

The value of the field of type double list.

CKDBRecordFieldEncryptedDoubleValue

The value of the encrypted field of type double.

