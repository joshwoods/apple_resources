

- StoreKit
-  SKCloudServiceSetupViewControllerDelegate Deprecated

Protocol

# SKCloudServiceSetupViewControllerDelegate

A protocol that defines the methods a cloud service setup view controller can use to get the status of the view, including when it is dismissed.

iOS 10.1–18.0DeprecatediPadOS 10.1–18.0DeprecatedMac Catalyst 13.1–18.0Deprecated

``` source
protocol SKCloudServiceSetupViewControllerDelegate : NSObjectProtocol
```

Deprecated

Use the musicSubscriptionOffer(isPresented:options:onLoadCompletion:) SwiftUI View Modifier from MusicKit

## Topics

### Receiving Notification of Dismissal

func cloudServiceSetupViewControllerDidDismiss(SKCloudServiceSetupViewController)

Tells the delegate that the cloud service setup view controller was dismissed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting a delegate

var delegate: (any SKCloudServiceSetupViewControllerDelegate)?

The cloud service view controller’s delegate.

Deprecated

