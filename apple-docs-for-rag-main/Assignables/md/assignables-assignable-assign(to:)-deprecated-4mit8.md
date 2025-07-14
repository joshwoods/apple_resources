

- Assignables
- Assignable
-  assign(to:) Deprecated

Instance Method

# assign(to:)

Assign this document to a user.

iOS 17.4–18.0DeprecatediPadOS 17.4–18.0DeprecatedMac Catalyst 17.4–18.0DeprecatedvisionOS

``` source
func assign(to userIdentity: some UserIdentity) throws -> AssignedWorkDocument
```

**Required** Default implementation provided.

Deprecated

Use makeAssignedWorkDocument() instead

## Parameters 

`userIdentity`  

The identity of the user to assign this document to.

## Return Value

A work document for the taker of the assignable document.

## Default Implementations

### Assignable Implementations

func assign(to: some UserIdentity) throws -> AssignedWorkDocument

Assign this document to a user.

## See Also

### Assigning a document

func assign(to: AnyUserIdentity) throws -> AssignedWorkDocument

Assign this document to a user.

**Required** Default implementation provided.

Deprecated

