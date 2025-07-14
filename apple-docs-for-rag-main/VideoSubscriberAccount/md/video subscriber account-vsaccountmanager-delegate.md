

- Video Subscriber Account
- VSAccountManager
-  delegate 

Instance Property

# delegate

The delegate of the account manager object.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
weak var delegate: (any VSAccountManagerDelegate)? { get set }
```

## Discussion

The system notifies the delegate when the app needs to present or dismiss authentication views, or decide whether to authenticate the user with their chosen provider.

The delegate must adopt the VSAccountManagerDelegate protocol.

## See Also

### Responding to Account Manager Requests

protocol VSAccountManagerDelegate

The methods you use to respond to authentication view controller requests.

