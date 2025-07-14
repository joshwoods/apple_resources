

- CKTool JS
-  CKDBPermissionType 

Enumeration

# CKDBPermissionType

The participant’s read and write permissions.

CKTool JS 1.2.15+

``` source
interface CKDBPermissionType {
 const string NONE;
 const string READ_ONLY;
 const string READ_WRITE;
 const string UNKNOWN;
};
```

## Overview

Possible values are `NONE`, `READ_ONLY`, `READ_WRITE`, and `UNKNOWN`.

```
import { CKDBPermissionType } from "@apple/cktool.database";
```

## Topics

### Enumeration Cases

NONE

READ_ONLY

READ_WRITE

UNKNOWN

## See Also

### Enumerations

CKDBQueryFilterType

An object that represents the type of a filter that indicates the comparison operator when applying the filter.

CKDBQuerySortOrder

An enumeration that represents the order to use when sorting records.

CKDBRecordReferenceAction

An object that represents the action to be performed for the referenced record.

CKDBShareAcceptanceStatus

An enumeration that indicates the status of accepting the shared record.

CKDBShareParticipantType

An enumeration that represents the type of a share participant.

