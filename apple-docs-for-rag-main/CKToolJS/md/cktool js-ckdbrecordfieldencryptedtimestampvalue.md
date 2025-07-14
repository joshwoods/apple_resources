

- CKTool JS
-  CKDBRecordFieldEncryptedTimestampValue 

Structure

# CKDBRecordFieldEncryptedTimestampValue

The value of the encrypted field of type timestamp.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldEncryptedTimestampValue {
 string type;
 date? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldEncryptedTimestampValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

A string in date-time format.

## See Also

### Timestamps

CKDBRecordFieldTimestampValue

The value of the field of type timestamp.

CKDBRecordFieldTimestampListValue

The value of the field of type timestamp list.

CKDBRecordFieldEncryptedTimestampListValue

The value of the encrypted field of type timestamp.

