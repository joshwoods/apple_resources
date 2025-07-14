

- CKTool JS
-  CKDBRecordFieldEncryptedBytesListValue 

Structure

# CKDBRecordFieldEncryptedBytesListValue

The value of the encrypted field of type bytes list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldEncryptedBytesListValue {
 string type;
 ByteArray[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldEncryptedBytesListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An array of strings, each containing a sequence of bytes.

## See Also

### Bytes

CKDBRecordFieldBytesValue

A field value that contains an array of bytes.

CKDBRecordFieldBytesListValue

A field value that contains an array of bytes.

CKDBRecordFieldEncryptedBytesValue

The value of the encrypted field of type bytes.

