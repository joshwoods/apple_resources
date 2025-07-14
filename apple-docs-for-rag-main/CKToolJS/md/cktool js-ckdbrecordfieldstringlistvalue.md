

- CKTool JS
-  CKDBRecordFieldStringListValue 

Structure

# CKDBRecordFieldStringListValue

The value of the field of type string list.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldStringListValue {
 string type;
 string[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldStringListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

An array of strings.

## See Also

### Strings

CKDBRecordFieldStringValue

The value of the field of type string.

CKDBRecordFieldEncryptedStringValue

The value of the encrypted field of type string.

CKDBRecordFieldEncryptedStringListValue

The value of the encrypted field of type string list.

