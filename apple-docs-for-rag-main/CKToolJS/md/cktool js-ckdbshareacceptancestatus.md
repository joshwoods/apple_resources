

- CKTool JS
-  CKDBShareAcceptanceStatus 

Enumeration

# CKDBShareAcceptanceStatus

An enumeration that indicates the status of accepting the shared record.

CKTool JS 1.2.15+

``` source
interface CKDBShareAcceptanceStatus {
 const string INVITED;
 const string ACCEPTED;
 const string REMOVED;
 const string UNSUBSCRIBED;
 const string UNKNOWN;
};
```

## Overview

Possible values are `INVITED`, `ACCEPTED`, `REMOVED`, and `UNKNOWN`.

```
import { CKDBShareAcceptanceStatus } from "@apple/cktool.database";
```

## Topics

### Enumeration Cases

ACCEPTED

INVITED

REMOVED

UNKNOWN

UNSUBSCRIBED

## See Also

### Enumerations

CKDBPermissionType

The participant’s read and write permissions.

CKDBQueryFilterType

An object that represents the type of a filter that indicates the comparison operator when applying the filter.

CKDBQuerySortOrder

An enumeration that represents the order to use when sorting records.

CKDBRecordReferenceAction

An object that represents the action to be performed for the referenced record.

CKDBShareParticipantType

An enumeration that represents the type of a share participant.

