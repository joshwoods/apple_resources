

- CloudKit
-  CKOperation 

Class

# CKOperation

The abstract base class for all operations that execute in a database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKOperation
```

## Mentioned in 

Encrypting User Data

Deciding whether CloudKit is right for your app

## Overview

All CloudKit operations descend from `CKOperation`, which provides the infrastructure for executing tasks in one of your app’s containers. Don’t subclass or create instances of this class directly. Instead, create instances of one of its concrete subclasses.

Use the properties of this class to configure the behavior of the operation before submitting it to a queue or executing it directly. CloudKit operations involve communicating with the iCloud servers to send and receive data. You can use the properties of this class to configure the behavior of those network requests to ensure the best performance for your app.

Important

`CKOperation` objects have a default quality of service level of QualityOfService.default (see qualityOfService). Operations with this service level are discretionary, and the system schedules them for an optimal time according to battery level and other factors. On iPhone, discretionary activities pause when the device is in Low Power Mode. For information about quality of service levels, see Prioritize Work with Quality of Service Classes in Energy Efficiency Guide for iOS Apps and Prioritize Work at the Task Level in Energy Efficiency Guide for Mac Apps.

### Long-Lived Operations

A *long-lived operation* is an operation that continues to run after the user closes the app. To specify a long-lived operation, set isLongLived to true, provide a completion handler, and execute the operation. To get the identifiers of all running long-lived operations, use the fetchAllLongLivedOperationIDsWithCompletionHandler: method that CKContainer provides. To get a specific long-lived operation, use the fetchLongLivedOperationWithID:completionHandler: method. Make sure you set the completion handler of a long-lived operation before you execute it so that the system can notify you when it completes and you can process the results. Do not execute an operation, change it to long-lived, and execute it again as a long-lived operation.

- Swift
- Objective-C

```
container.fetchAllLongLivedOperationIDs(completionHandler: { (operationIDs, error) in
    if let error = error {
        print("Error fetching long lived operations: \(error)")
        // Handle error
        return
    }
    guard let identifiers = operationIDs else { return }
    for operationID in identifiers {
        container.fetchLongLivedOperation(withID: operationID, completionHandler: { (operation, error) in
            if let error = error {
                print("Error fetching operation: \(operationID)\n\(error)")
                // Handle error
                return
            }
            guard let operation = operation else { return }
            // Add callback handlers to operation
            container.add(operation)
        })
    }
})
```

```
[container fetchAllLongLivedOperationIDsWithCompletionHandler:^(NSArray *_Nullable operationIDs, NSError *_Nullable error) {
    if (error) {
        // Handle error
        return
    }
    for (NSString *operationID in operationIDs) {
        [container fetchLongLivedOperationWithID:operationID completionHandler:^(CKOperation *_Nullable operation, NSError *_Nullable error) {
            if (error) {
                // Handle error
                return
            }
            // Add callback handlers to operation
            [container addOperation:operation];
        }];
    }
}];
```

The following is the typical life cycle of a long-lived operation:

1.  The app creates a long-lived operation and executes it.

The daemon starts saving and sending the callbacks to the running app. 2. The app exits.

The daemon continues running the long-lived operation and saves the callbacks. 3. The app launches and fetches the long-lived operation.

If the operation is running or if it completed within the previous 24 hours, the daemon returns a proxy for the long-lived operation. If the operation completed more than 24 hours previously, the daemon may stop returning it in fetch requests. 4. The app runs the long-lived operation again.

The daemon sends the app all the saved callbacks (it doesn’t actually rerun the operation), and continues saving the callbacks and sending them to the running app. 5. The app receives the completion callback or the app cancels the operation.

The daemon stops including the operation in future fetch results.

## Topics

### Creating an Operation

init()

Creates an operation.

### Identifying the Operation

var operationID: CKOperation.ID

A unique identifier for a long-lived operation.

typealias ID

A type that represents the ID of an operation.

### Managing the Operation’s Configuration

var configuration: CKOperation.Configuration!

The operation’s configuration.

class Configuration

An object that describes how a CloudKit operation behaves.

var group: CKOperationGroup?

The operation’s group.

var longLivedOperationWasPersistedBlock: (() -> Void)?

The closure to execute when the server begins to store callbacks for the long-lived operation.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- Operation

### Inherited By

- CKAcceptSharesOperation
- CKDatabaseOperation
- CKDiscoverAllUserIdentitiesOperation
- CKDiscoverUserIdentitiesOperation
- CKFetchShareMetadataOperation
- CKFetchShareParticipantsOperation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

