

- Assignables
- AnonymousUserIdentity
-  scope(\_:) 

Instance Method

# scope(\_:)

Sets the user identity for document-related operations that occur within the async closure passed in.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@discardableResult
func scope(_ access: () async throws -> R) async rethrows -> R
```

## Parameters 

`access`  

An async closure containing document-related operations . Operations in the closure will be attributed to this user identity.

## Return Value

The result of the closure.

