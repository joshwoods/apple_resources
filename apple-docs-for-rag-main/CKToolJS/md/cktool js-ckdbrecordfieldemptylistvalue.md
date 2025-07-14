

- CKTool JS
-  CKDBRecordFieldEmptyListValue 

Structure

# CKDBRecordFieldEmptyListValue

The value of the field of type empty list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldEmptyListValue {
 string type;
 string[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldEmptyListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An empty array.

