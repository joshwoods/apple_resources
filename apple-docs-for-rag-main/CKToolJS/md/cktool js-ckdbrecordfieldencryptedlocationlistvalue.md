

- CKTool JS
-  CKDBRecordFieldEncryptedLocationListValue 

Structure

# CKDBRecordFieldEncryptedLocationListValue

The value of the encrypted field of type location list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldEncryptedLocationListValue {
 string type;
 CKDBLocation[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldEncryptedLocationListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An array of location objects.

## See Also

### Locations

CKDBRecordFieldLocationValue

The value of the field of type location.

CKDBRecordFieldLocationListValue

The value of the field of type location list.

CKDBRecordFieldEncryptedLocationValue

The value of the encrypted field of type location.

