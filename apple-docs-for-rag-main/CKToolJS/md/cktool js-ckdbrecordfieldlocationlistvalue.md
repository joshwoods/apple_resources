

- CKTool JS
-  CKDBRecordFieldLocationListValue 

Structure

# CKDBRecordFieldLocationListValue

The value of the field of type location list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldLocationListValue {
 string type;
 CKDBLocation[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldLocationListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An array of values, each containing a location coordinates.

## See Also

### Locations

CKDBRecordFieldLocationValue

The value of the field of type location.

CKDBRecordFieldEncryptedLocationValue

The value of the encrypted field of type location.

CKDBRecordFieldEncryptedLocationListValue

The value of the encrypted field of type location list.

