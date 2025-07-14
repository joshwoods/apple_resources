

- Network Extension
- NEAppPushManager
-  delegate 

Instance Property

# delegate

A delegate that receives incoming call information from the provider.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
weak var delegate: (any NEAppPushDelegate)? { get set }
```

## See Also

### Working with a delegate

protocol NEAppPushDelegate

A protocol that defines how an app push manager instance interacts with the framework.

