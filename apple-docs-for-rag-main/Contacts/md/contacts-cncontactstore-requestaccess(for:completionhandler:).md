

- Contacts
- CNContactStore
-  requestAccess(for:completionHandler:) 

Instance Method

# requestAccess(for:completionHandler:)

Requests access to the user’s contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func requestAccess(
    for entityType: CNEntityType,
    completionHandler: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func requestAccess(for entityType: CNEntityType) async throws -> Bool
```

## Parameters 

`entityType`  

Set to `CNEntityTypeContacts`.

`completionHandler`  

Set granted to true if the user allows access and error is `nil`.

## Mentioned in 

Accessing the contact store

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestAccess(for entityType: CNEntityType) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Users grant or deny access to contact data on a per-app basis. Request access to contact data by calling the requestAccess(for:completionHandler:) method, which returns right away. The first time your app calls this method, the system prompts the user to grant or deny access to your app. The system then saves the user’s response and does not prompt them again.

The system executes `completionHandler` on an arbitrary queue. It is recommended that you use CNContactStore instance methods in this completion handler instead of the UI main thread. This method is optional when CNContactStore is used in the background thread. If you don’t request access, CNContactStore may block your app while asking the user for access.

## See Also

### Requesting access to the user’s contacts

class func authorizationStatus(for: CNEntityType) -> CNAuthorizationStatus

Returns the current authorization status to access the contact data.

enum CNAuthorizationStatus

An authorization status the user can grant for an app to access the specified entity type.

enum CNEntityType

The entities the user can grant access to.

