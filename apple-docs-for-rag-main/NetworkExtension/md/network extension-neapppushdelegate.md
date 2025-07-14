

- Network Extension
-  NEAppPushDelegate 

Protocol

# NEAppPushDelegate

A protocol that defines how an app push manager instance interacts with the framework.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
protocol NEAppPushDelegate : NSObjectProtocol
```

## Topics

### Receiving calls

func appPushManager(NEAppPushManager, didReceiveIncomingCallWithUserInfo: [AnyHashable : Any])

A delegate method that the framework invokes when the provider reports an incoming call.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working with a delegate

var delegate: (any NEAppPushDelegate)?

A delegate that receives incoming call information from the provider.

