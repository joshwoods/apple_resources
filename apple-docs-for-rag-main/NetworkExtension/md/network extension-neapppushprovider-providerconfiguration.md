

- Network Extension
- NEAppPushProvider
-  providerConfiguration 

Instance Property

# providerConfiguration

A dictionary that contains current vendor-specific configuration parameters.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var providerConfiguration: [String : Any]? { get }
```

## Mentioned in 

Maintaining a Reliable Network Connection

## Discussion

The NEAppPushManager provides this dictionary. Use key-value observing to watch for changes in the dictionary.

