

- RealityKit
- MultipeerConnectivityService
-  startSync() 

Instance Method

# startSync()

Begins multipeer synchronization.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
func startSync()
```

## Discussion

Call this method to restart multipeer syncing with connected peers after calling stopSync(). You don’t need to call this method to begin syncing. RealityKit calls this method automatically when you assign a MultipeerConnectivityService to a Scene.

## See Also

### Pausing and resuming

func stopSync()

Stops multipeer synchronization.

