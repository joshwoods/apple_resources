

- CKTool JS
-  CKDBRecordFieldBytesValue 

Structure

# CKDBRecordFieldBytesValue

A field value that contains an array of bytes.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldBytesValue {
 string type;
 ByteArray? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldBytesValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

The array of bytes this field contains.

## See Also

### Bytes

CKDBRecordFieldBytesListValue

A field value that contains an array of bytes.

CKDBRecordFieldEncryptedBytesValue

The value of the encrypted field of type bytes.

CKDBRecordFieldEncryptedBytesListValue

The value of the encrypted field of type bytes list.

