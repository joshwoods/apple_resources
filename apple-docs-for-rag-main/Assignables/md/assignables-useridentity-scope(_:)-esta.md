

- Assignables
- UserIdentity
-  scope(\_:) 

Instance Method

# scope(\_:)

Sets the user identity for document-related operations that occur within the closure passed in.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@discardableResult
func scope(_ access: () throws -> R) rethrows -> R
```

## Parameters 

`access`  

A closure containing document-related operations . Operations in the closure will be attributed to this user identity.

## Return Value

The result of the closure.

## See Also

### Setting the scope

func scope&lt;R>(() async throws -> R) async rethrows -> R

Sets the user identity for document-related operations that occur within the async closure passed in.

