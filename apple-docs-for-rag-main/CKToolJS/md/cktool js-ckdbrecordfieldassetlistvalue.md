

- CKTool JS
-  CKDBRecordFieldAssetListValue 

Structure

# CKDBRecordFieldAssetListValue

A field value that contains an array of assets.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldAssetListValue {
 string type;
 CKDBAsset[]? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldAssetListValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

The array of asset objects in this record field.

## See Also

### Assets

CKDBRecordFieldAssetValue

The value of the field of the type asset.

