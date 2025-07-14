

- Contacts
- CNContactStore
-  authorizationStatus(for:) 

Type Method

# authorizationStatus(for:)

Returns the current authorization status to access the contact data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func authorizationStatus(for entityType: CNEntityType) -> CNAuthorizationStatus
```

## Parameters 

`entityType`  

Set to CNEntityType.

## Mentioned in 

Accessing the contact store

## Return Value

The current authorization status to access the contact data.

## Discussion

Based on the authorization status, your application might display or hide its UI elements that access any Contacts API. This method is thread-safe and will not block your application. To see different authorization status, see `CNAuthorizationStatus`.

## See Also

### Requesting access to the user’s contacts

func requestAccess(for: CNEntityType, completionHandler: (Bool, (any Error)?) -> Void)

Requests access to the user’s contacts.

enum CNAuthorizationStatus

An authorization status the user can grant for an app to access the specified entity type.

enum CNEntityType

The entities the user can grant access to.

