

- CKTool JS
-  CKDBRecordFieldEncryptedLocationValue 

Structure

# CKDBRecordFieldEncryptedLocationValue

The value of the encrypted field of type location.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldEncryptedLocationValue {
 string type;
 CKDBLocation? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldEncryptedLocationValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

## See Also

### Locations

CKDBRecordFieldLocationValue

The value of the field of type location.

CKDBRecordFieldLocationListValue

The value of the field of type location list.

CKDBRecordFieldEncryptedLocationListValue

The value of the encrypted field of type location list.

