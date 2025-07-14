

- StoreKit
- SKCloudServiceSetupViewController
-  delegate Deprecated

Instance Property

# delegate

The cloud service view controller’s delegate.

iOS 10.1–18.0DeprecatediPadOS 10.1–18.0DeprecatedMac Catalyst 13.1–18.0Deprecated

``` source
@MainActor
weak var delegate: (any SKCloudServiceSetupViewControllerDelegate)? { get set }
```

Deprecated

Use the musicSubscriptionOffer(isPresented:options:onLoadCompletion:) SwiftUI View Modifier from MusicKit

## Discussion

You can identify a delegate to get informed when the cloud service setup view controller is dismissed.

## See Also

### Setting a delegate

protocol SKCloudServiceSetupViewControllerDelegate

A protocol that defines the methods a cloud service setup view controller can use to get the status of the view, including when it is dismissed.

Deprecated

