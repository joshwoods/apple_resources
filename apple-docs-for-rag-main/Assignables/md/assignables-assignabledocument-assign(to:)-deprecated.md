

- Assignables
- AssignableDocument
-  assign(to:) Deprecated

Instance Method

# assign(to:)

Assign this document to a user.

iOS 17.4–18.0DeprecatediPadOS 17.4–18.0DeprecatedMac Catalyst 17.4–18.0DeprecatedvisionOS

``` source
func assign(to userIdentity: AnyUserIdentity) throws -> AssignedWorkDocument
```

Deprecated

Use makeAssignedWorkDocument() instead

## Parameters 

`userIdentity`  

The identity of the user to assign this document to.

## Return Value

A work document for the taker of the assignable document.

