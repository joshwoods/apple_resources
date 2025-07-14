

- HomeKit
- HMNetworkConfigurationProfile
-  delegate 

Instance Property

# delegate

A delegate that HomeKit tells about changes in the state of network access.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
weak var delegate: (any HMNetworkConfigurationProfileDelegate)? { get set }
```

## See Also

### Listening for access changes

protocol HMNetworkConfigurationProfileDelegate

An interface that your app adopts to receive notifications about changes in the state of network access.

