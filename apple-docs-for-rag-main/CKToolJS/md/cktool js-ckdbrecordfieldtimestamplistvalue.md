

- CKTool JS
-  CKDBRecordFieldTimestampListValue 

Structure

# CKDBRecordFieldTimestampListValue

The value of the field of type timestamp list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldTimestampListValue {
 string type;
 Date[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldTimestampListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An array of strings in date-time format.

## See Also

### Timestamps

CKDBRecordFieldTimestampValue

The value of the field of type timestamp.

CKDBRecordFieldEncryptedTimestampValue

The value of the encrypted field of type timestamp.

CKDBRecordFieldEncryptedTimestampListValue

The value of the encrypted field of type timestamp.

