

- HomeKit
- HMAccessoryBrowser
-  delegate 

Instance Property

# delegate

A delegate that receives updates on the discovered accessories.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
weak var delegate: (any HMAccessoryBrowserDelegate)? { get set }
```

## See Also

### Tracking the addition or removal of accessories

protocol HMAccessoryBrowserDelegate

An interface used to notify an accessory browser delegate of new accessories.

