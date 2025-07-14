

- CKTool JS
-  CKDBRecordFieldAssetValue 

Structure

# CKDBRecordFieldAssetValue

The value of the field of the type asset.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordFieldAssetValue {
 string type;
 CKDBAsset? value;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordFieldAssetValue } from "@apple/cktool.database";
```

## Topics

### Instance Properties

type

A string used to identify the field type.

value

## See Also

### Assets

CKDBRecordFieldAssetListValue

A field value that contains an array of assets.

