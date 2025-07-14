

- CloudKit
- CKQuerySubscription
- CKQuerySubscription.Options
-  firesOnRecordDeletion 

Type Property

# firesOnRecordDeletion

An option that instructs CloudKit to send a push notification when it deletes a record that matches a subscription’s criteria.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
static var firesOnRecordDeletion: CKQuerySubscription.Options { get }
```

## See Also

### Accessing Subscription Options

static var firesOnRecordCreation: CKQuerySubscription.Options

An option that instructs CloudKit to send a push notification when it creates a record that matches a subscription’s criteria.

static var firesOnRecordUpdate: CKQuerySubscription.Options

An option that instructs CloudKit to send a push notification when it modifies a record that matches a subscription’s criteria.

static var firesOnce: CKQuerySubscription.Options

An option that instructs CloudKit to send a push notification only once.

