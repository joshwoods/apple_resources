

- CKTool JS
-  CKDBRecordFieldReferenceValue 

Structure

# CKDBRecordFieldReferenceValue

The value of the field of type reference.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldReferenceValue {
 string type;
 CKDBRecordReference? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldReferenceValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

## See Also

### References

CKDBRecordFieldReferenceListValue

The value of the field of type reference list.

