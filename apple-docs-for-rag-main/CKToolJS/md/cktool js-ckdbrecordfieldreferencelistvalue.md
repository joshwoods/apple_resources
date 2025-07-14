

- CKTool JS
-  CKDBRecordFieldReferenceListValue 

Structure

# CKDBRecordFieldReferenceListValue

The value of the field of type reference list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldReferenceListValue {
 string type;
 CKDBRecordReference[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldReferenceListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

The array of values, each containing a reference to a CloudKit record

## See Also

### References

CKDBRecordFieldReferenceValue

The value of the field of type reference.

