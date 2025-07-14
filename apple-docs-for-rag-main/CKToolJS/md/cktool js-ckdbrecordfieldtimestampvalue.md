

- CKTool JS
-  CKDBRecordFieldTimestampValue 

Structure

# CKDBRecordFieldTimestampValue

The value of the field of type timestamp.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldTimestampValue {
 string type;
 date? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldTimestampValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

A string in date-time format.

## See Also

### Timestamps

CKDBRecordFieldTimestampListValue

The value of the field of type timestamp list.

CKDBRecordFieldEncryptedTimestampValue

The value of the encrypted field of type timestamp.

CKDBRecordFieldEncryptedTimestampListValue

The value of the encrypted field of type timestamp.

