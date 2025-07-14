

- CKTool JS
-  CKDBShareParticipantType 

Enumeration

# CKDBShareParticipantType

An enumeration that represents the type of a share participant.

CKTool JS 1.2.15+

``` source
interface CKDBShareParticipantType {
 const string OWNER;
 const string ADMINISTRATOR;
 const string USER;
 const string PUBLIC_USER;
 const string UNKNOWN;
};
```

## Overview

Possible values are `OWNER`, `ADMINISTRATOR`, `USER`, `PUBLIC_USER`, and `UNKNOWN`.

```
import { CKDBShareParticipantType } from "@apple/cktool.database";
```

## Topics

### Enumeration Cases

ADMINISTRATOR

OWNER

PUBLIC_USER

UNKNOWN

USER

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

CKDBShareAcceptanceStatus

An enumeration that indicates the status of accepting the shared record.

