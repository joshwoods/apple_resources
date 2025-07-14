

- Video Subscriber Account
- VSAccountManagerDelegate
-  accountManager(\_:dismiss:) 

Instance Method

# accountManager(\_:dismiss:)

Tells the delegate to dismiss an authentication view controller.

iOS 10.0+iPadOS 10.0+tvOS 10.0+visionOS 1.0+

``` source
func accountManager(
    _ accountManager: VSAccountManager,
    dismiss viewController: UIViewController
)
```

**Required**

## Parameters 

`accountManager`  

The account manager instance that requests to dismiss the authentication view controller.

`viewController`  

The view controller that your app must dismiss.

## Discussion

The system calls this method when the `VideoSubscriberAccount` framework requires your app to dismiss an authentication view controller. You must use dismiss(animated:completion:) to dismiss the view controller before returning from this method.

