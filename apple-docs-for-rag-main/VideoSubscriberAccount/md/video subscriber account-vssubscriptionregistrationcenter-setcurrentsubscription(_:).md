

- Video Subscriber Account
- VSSubscriptionRegistrationCenter
-  setCurrentSubscription(\_:) 

Instance Method

# setCurrentSubscription(\_:)

Sets the subscription information for the current user.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedmacOStvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func setCurrentSubscription(_ currentSubscription: VSSubscription?)
```

## Parameters 

`currentSubscription`  

A VSSubscription object that contains the subscription information to set.

## Discussion

Your app uses this method to set a subscription when the subscriber first authenticates or when their subscription changes.

When the subscriber signs out or loses access to subscription content, your app calls this method with a value of `nil`.

Call this method as needed to update the subscription, such as when you confirm the validity of the subscription, or in response to app lifecycle events when your app becomes active. The system can use this activity as a hint that the user is actively using the subscription.

The system throws an exception if you try to set the current subscription to an unknown access level. Don’t set a subscription if the user only has access to free content.

