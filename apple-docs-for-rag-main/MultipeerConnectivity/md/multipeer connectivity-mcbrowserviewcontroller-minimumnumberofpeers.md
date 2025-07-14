

- Multipeer Connectivity
- MCBrowserViewController
-  minimumNumberOfPeers 

Instance Property

# minimumNumberOfPeers

The minimum number of peers that need to be in a session, including the local peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var minimumNumberOfPeers: Int { get set }
```

## Discussion

The smallest allowable value (and the default) is 2.

## See Also

### Getting and Setting the Maximum and Minimum Number of Peers

var maximumNumberOfPeers: Int

The maximum number of peers allowed in a session, including the local peer.

