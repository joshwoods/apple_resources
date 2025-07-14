

- CloudKit
-  CKDiscoverAllUserIdentitiesOperation Deprecated

Class

# CKDiscoverAllUserIdentitiesOperation

An operation that uses the device’s contacts to search for discoverable iCloud users.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
class CKDiscoverAllUserIdentitiesOperation
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Overview

Use this operation to discover iCloud users that match entries in the device’s Contacts database. CloudKit uses the email addresses and phone numbers in each Contact record to search for a matching iCloud account.

Although your app doesn’t need authorization to use the Contacts database to execute this operation, if it has authorization, you can use the contactIdentifiers property on any returned user identity to fetch the corresponding Contact record from the database.

Note

This operation scales linearly with the number of email addresses and phone numbers in the device’s Contacts database, and may take some time to complete.

Before CloudKit can return a user’s identity, you must ask for their permission by calling requestApplicationPermission(_:completionHandler:). Do this as part of any onboarding where you can highlight the benefits of being discoverable within the context of your app.

The operation executes the handlers you provide on an internal queue it manages. Your handlers must be capable of executing on a background queue. Tasks that need access to the main queue must redirect as appropriate.

The operation calls discoverAllUserIdentitiesCompletionBlock after it executes and returns results. Use the completion handler to perform housekeeping tasks for the operation. It should also manage any failures, whether due to an error or an explicit cancellation.

Note

Because this class inherits from Operation, you can also set the completionBlock property. The operation calls both completion handlers if they’re both set.

CloudKit operations have a default QoS of QualityOfService.default. Operations with this service level are discretionary. The system schedules their execution at an optimal time according to battery level and network conditions, among other factors. Use the qualityOfService property to set a more appropriate QoS for the operation.

The following example shows how to create the operation, configure its callbacks, and execute it using the default container’s queue:

```
func fetchUserIdentities(
    completion: @escaping (Result) -> Void) {

    var identities = [CKUserIdentity]()

    // Create an operation to discover all the iCloud users
    // in the user's Contacts database that use the app, and
    // opt in to being discoverable.
    let operation = CKDiscoverAllUserIdentitiesOperation()

    // Cache the user identities as CloudKit discovers them.  
    operation.userIdentityDiscoveredBlock = { userIdentity in
        identities.append(userIdentity)
    }

    // If the operation fails, return the error to the caller.
    // Otherwise, return the array of discovered user identities.
    operation.discoverAllUserIdentitiesCompletionBlock = { error in
        if let error = error {
            completion(.failure(error))
        } else {
            completion(.success(identities))
        }
    }

    // Set an appropriate QoS and add the operation to the
    // default container's queue to execute it.
    operation.qualityOfService = .userInitiated
    CKContainer.default().add(operation)
}
```

## Topics

### Creating an Operation

init()

Creates an operation for searching the device’s contacts.

### Processing the Operation Results

var userIdentityDiscoveredBlock: ((CKUserIdentity) -> Void)?

The closure to execute for each user identity.

var discoverAllUserIdentitiesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

### Instance Properties

var discoverAllUserIdentitiesResultBlock: ((Result&lt;Void, any Error>) -> Void)?

## Relationships

### Inherits From

- CKOperation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Deprecated classes

class CKDiscoverUserIdentitiesOperation

An operation that uses the provided criteria to search for discoverable iCloud users.

Deprecated

class CKFetchRecordChangesOperation

An operation that reports on the changed and deleted records in the specified record zone.

Deprecated

