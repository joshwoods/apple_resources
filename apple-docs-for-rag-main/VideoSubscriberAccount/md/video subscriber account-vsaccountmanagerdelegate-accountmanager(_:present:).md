

- Video Subscriber Account
- VSAccountManagerDelegate
-  accountManager(\_:present:) 

Instance Method

# accountManager(\_:present:)

Tells the delegate to present an authentication view controller.

iOS 10.0+iPadOS 10.0+tvOS 10.0+visionOS 1.0+

``` source
func accountManager(
    _ accountManager: VSAccountManager,
    present viewController: UIViewController
)
```

**Required**

## Parameters 

`accountManager`  

The account manager instance that requests the authentication view controller.

`viewController`  

The view controller your app must present to the user.

## Discussion

The system calls this method when the `VideoSubscriberAccount` framework requires your app to present an authentication view controller. You must use present(_:animated:completion:) to present the view controller before returning from this method.

