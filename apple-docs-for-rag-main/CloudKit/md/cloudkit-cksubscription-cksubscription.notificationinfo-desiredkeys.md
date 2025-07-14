

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  desiredKeys 

Instance Property

# desiredKeys

The names of fields to include in the push notification’s payload.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
var desiredKeys: [CKRecord.FieldKey]? { get set }
```

## Discussion

This property contains an array of strings, each of which corresponds to the name of a field in the record that triggers the notification. When the system receives a notification, it includes the keys and their corresponding values. You can request a maximum of three keys.

For the keys you specify, the allowable types are NSString, NSNumber, CLLocation, NSDate, and CKRecord.Reference. You can’t specify keys with values that contain other data types. CloudKit may truncate strings that are more than 100 characters when it adds them to the notification’s payload.

