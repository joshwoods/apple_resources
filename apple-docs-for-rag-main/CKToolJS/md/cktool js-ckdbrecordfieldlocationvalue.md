

- CKTool JS
-  CKDBRecordFieldLocationValue 

Structure

# CKDBRecordFieldLocationValue

The value of the field of type location.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldLocationValue {
 string type;
 CKDBLocation? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldLocationValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

## See Also

### Locations

CKDBRecordFieldLocationListValue

The value of the field of type location list.

CKDBRecordFieldEncryptedLocationValue

The value of the encrypted field of type location.

CKDBRecordFieldEncryptedLocationListValue

The value of the encrypted field of type location list.

