

- CKTool JS
-  CKDBQueryFilterType 

Enumeration

# CKDBQueryFilterType

An object that represents the type of a filter that indicates the comparison operator when applying the filter.

CKTool JS 1.2.15+

``` source
interface CKDBQueryFilterType {
 const string EQUALS;
 const string NOT_EQUALS;
 const string LESS_THAN;
 const string LESS_THAN_OR_EQUALS;
 const string GREATER_THAN;
 const string GREATER_THAN_OR_EQUALS;
 const string NEAR;
 const string CONTAINS_ALL_TOKENS;
 const string IN;
 const string NOT_IN;
 const string CONTAINS_ANY_TOKENS;
 const string LIST_CONTAINS;
 const string LIST_NOT_CONTAINS;
 const string LIST_CONTAINS_ANY;
 const string LIST_NOT_CONTAINS_ANY;
 const string BEGINS_WITH;
 const string NOT_BEGINS_WITH;
 const string LIST_MEMBER_BEGINS_WITH;
 const string NOT_LIST_MEMBER_BEGINS_WITH;
 const string LIST_CONTAINS_ALL;
 const string NOT_LIST_CONTAINS_ALL;
};
```

## Overview

```
import { CKDBQueryFilterType } from "@apple/cktool.database";
```

## Topics

### Enumeration Cases

BEGINS_WITH

CONTAINS_ALL_TOKENS

CONTAINS_ANY_TOKENS

EQUALS

GREATER_THAN

GREATER_THAN_OR_EQUALS

IN

LESS_THAN

LESS_THAN_OR_EQUALS

LIST_CONTAINS

LIST_CONTAINS_ALL

LIST_CONTAINS_ANY

LIST_MEMBER_BEGINS_WITH

LIST_NOT_CONTAINS

LIST_NOT_CONTAINS_ANY

NEAR

NOT_BEGINS_WITH

NOT_EQUALS

NOT_IN

NOT_LIST_CONTAINS_ALL

NOT_LIST_MEMBER_BEGINS_WITH

## See Also

### Enumerations

CKDBPermissionType

The participant’s read and write permissions.

CKDBQuerySortOrder

An enumeration that represents the order to use when sorting records.

CKDBRecordReferenceAction

An object that represents the action to be performed for the referenced record.

CKDBShareAcceptanceStatus

An enumeration that indicates the status of accepting the shared record.

CKDBShareParticipantType

An enumeration that represents the type of a share participant.

