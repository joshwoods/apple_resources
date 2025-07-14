

- CloudKit
-  CKDiscoverUserIdentitiesOperation Deprecated

Class

# CKDiscoverUserIdentitiesOperation

An operation that uses the provided criteria to search for discoverable iCloud users.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
class CKDiscoverUserIdentitiesOperation
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Overview

Use this operation to discover one or more iCloud users that match identity information you provide, such as email addresses and phone numbers.

Before CloudKit can return a user’s identity, you must ask for their permission by calling requestApplicationPermission(_:completionHandler:). Do this as part of any onboarding where you can highlight the benefits of being discoverable within the context of your app.

The operation executes the handlers you provide on an internal queue it manages. Your handlers must be capable of executing on a background queue. Tasks that need access to the main queue must redirect as appropriate.

The operation calls discoverUserIdentitiesCompletionBlock after it executes and returns results. Use the completion handler to perform housekeeping tasks for the operation. It should also manage any failures, whether due to an error or an explicit cancellation.

Note

Because this class inherits from Operation, you can also set the completionBlock property. The operation calls both completion handlers if they’re both set.

CloudKit operations have a default QoS of QualityOfService.default. Operations with this service level are discretionary. The system schedules their execution at an optimal time according to battery level and network conditions, among other factors. Use the qualityOfService property to set a more appropriate QoS for the operation.

The following example shows how to create the operation, configure its callbacks, and execute it using the default container’s queue:

```
func fetchUserIdentities(withEmails emails: [String],
    completion: @escaping (Result) -> Void) {

    var identities = [CKUserIdentity]()

    // Convert the email addresses into instances of
    // CKUserIdentity.LookupInfo, which CloudKit uses
    // to discover identities.
    let lookupInfos =
        CKUserIdentity.LookupInfo.lookupInfos(withEmails: emails)

    // Create the operation using the array of lookup objects.
    let operation = CKDiscoverUserIdentitiesOperation(
        userIdentityLookupInfos: lookupInfos)

    // Cache the user identities as CloudKit discovers them.
    operation.userIdentityDiscoveredBlock = { userIdentity, _ in
        identities.append(userIdentity)
    }

    // If the operation fails, return the error to the caller.
    // Otherwise, return the array of discovered user identities.
    operation.discoverUserIdentitiesCompletionBlock = { error in
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

Creates an operation for discovering user identities.

convenience init(userIdentityLookupInfos: [CKUserIdentity.LookupInfo])

Creates an operation for discovering the user identities of the specified lookup infos.

### Configuring the Operation

var userIdentityLookupInfos: [CKUserIdentity.LookupInfo]

The lookup info for discovering user identities.

### Processing the Results

var userIdentityDiscoveredBlock: ((CKUserIdentity, CKUserIdentity.LookupInfo) -> Void)?

The closure to execute for each user identity.

var discoverUserIdentitiesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

### Instance Properties

var discoverUserIdentitiesResultBlock: ((Result&lt;Void, any Error>) -> Void)?

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

class CKDiscoverAllUserIdentitiesOperation

An operation that uses the device’s contacts to search for discoverable iCloud users.

Deprecated

class CKFetchRecordChangesOperation

An operation that reports on the changed and deleted records in the specified record zone.

Deprecated

