

- CloudKit JS
-  CloudKit.QueryFilterComparator 

Enumeration

# CloudKit.QueryFilterComparator

The comparators you use to create queries.

CloudKit JS 1.0+

``` source
interface CloudKit.QueryFilterComparator {
 const String EQUALS;
 const String NOT_EQUALS;
 const String LESS_THAN;
 const String LESS_THAN_OR_EQUALS;
 const String GREATER_THAN;
 const String GREATER_THAN_OR_EQUALS;
 const String NEAR;
 const String CONTAINS_ALL_TOKENS;
 const String IN;
 const String NOT_IN;
 const String CONTAINS_ANY_TOKENS;
 const String LIST_CONTAINS;
 const String LIST_CONTAINS_ANY;
 const String NOT_LIST_CONTAINS;
 const String NOT_LIST_CONTAINS_ANY;
 const String BEGINS_WITH;
 const String NOT_BEGINS_WITH;
 const String LIST_MEMBER_BEGINS_WITH;
 const String NOT_LIST_MEMBER_BEGINS_WITH;
 const String LIST_CONTAINS_ALL;
 const String NOT_LIST_CONTAINS_ALL;
};
```

## Topics

### Enumeration Cases

BEGINS_WITH

Finds records with a string field that begins with a substring.

CONTAINS_ALL_TOKENS

Finds records with text fields containing all tokens.

CONTAINS_ANY_TOKENS

Finds records with text fields containing any token.

EQUALS

The value on the left is equal to the value on the right.

GREATER_THAN

The value on the left is greater than the value on the right.

GREATER_THAN_OR_EQUALS

The value on the left is greater than or equal to the value on the right.

IN

The value on the left is in the list on the right.

LESS_THAN

The value on the left is less than the value on the right.

LESS_THAN_OR_EQUALS

The value on the left is less than or equal to the value on the right.

LIST_CONTAINS

Finds records containing values in its list field.

LIST_CONTAINS_ALL

Finds records containing all values in its list field.

LIST_CONTAINS_ANY

Finds records that contain any of the values in its list field.

LIST_MEMBER_BEGINS_WITH

Finds records containing a value as the first item in its list field.

NEAR

The location on the left is within the specified distance of the location on the right.

NOT_BEGINS_WITH

Finds records with a string field that doesn’t begin with a substring.

NOT_EQUALS

The value on the left is not equal to the value on the right.

NOT_IN

The value on the left is not in the list on the right.

NOT_LIST_CONTAINS

Finds records not containing values not in its list field.

NOT_LIST_CONTAINS_ALL

Finds records not containing all values in its list field.

NOT_LIST_CONTAINS_ANY

Finds records not containing any of the values in its list field.

NOT_LIST_MEMBER_BEGINS_WITH

Finds records not containing a value as the first item in its list field.

## See Also

### Enumerations

CloudKit.AppleIDButtonTheme

Specifies the look of the Apple ID button.

CloudKit.DatabaseScope

Available database scopes.

CloudKit.ReferenceAction

The delete action for a reference object.

CloudKit.ShareParticipantAcceptanceStatus

The status of a participant accepting a share invitation.

CloudKit.ShareParticipantPermission

The status of a participant accepting a share invitation.

CloudKit.ShareParticipantType

Determines whether a participant can modify the list of participants of a shared record.

CloudKit.SubscriptionType

The type of subscription.

