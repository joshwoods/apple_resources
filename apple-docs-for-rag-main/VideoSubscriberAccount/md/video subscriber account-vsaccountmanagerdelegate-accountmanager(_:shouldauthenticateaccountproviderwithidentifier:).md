

- Video Subscriber Account
- VSAccountManagerDelegate
-  accountManager(\_:shouldAuthenticateAccountProviderWithIdentifier:) 

Instance Method

# accountManager(\_:shouldAuthenticateAccountProviderWithIdentifier:)

Asks the delegate whether to authenticate the user with the selected provider.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
optional func accountManager(
    _ accountManager: VSAccountManager,
    shouldAuthenticateAccountProviderWithIdentifier accountProviderIdentifier: String
) -> Bool
```

## Parameters 

`accountManager`  

The account manager instance that requests the authentication view controller.

`accountProviderIdentifier`  

The supported account provider the user has selected.

## Return Value

Return true to attempt authentication with the selected provider; otherwise, return false to respond with an unsupported provider error.

## Discussion

The system calls this method when the user chooses a provider from the list of supported providers; it isn’t called if the user selects “Other TV Providers”. Use this method to temporarily refrain from authenticating the user with the supported provider during a brief outage or service degradation.

If you don’t implement this method, the user can authenticate with all supported providers.

