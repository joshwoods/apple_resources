

- AVFAudio
- AVAudioSession
-  prepareRouteSelectionForPlayback(completionHandler:) 

Instance Method

# prepareRouteSelectionForPlayback(completionHandler:)

Prepares the route selection for long-form video playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func prepareRouteSelectionForPlayback(completionHandler: @escaping (Bool, AVAudioSession.RouteSelection) -> Void)
```

``` source
func prepareRouteSelectionForPlayback() async -> (Bool, AVAudioSession.RouteSelection)
```

## Parameters 

`completionHandler`  

A completion handler called after the system finishes preparing the playback route. The system passes the completion handler the following parameters:

`shouldStartPlayback`  
A Boolean value that indicates whether playback should start.

`routeSelection`  
A route selection value that indicates the active playback route.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func prepareRouteSelectionForPlayback() async -> (Bool, AVAudioSession.RouteSelection)
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

When playing long-form video content, call this method to indicate that playback is about to begin. Doing so provides the system the opportunity to prompt the user for an output destination, if needed, and perform any required routing.

The system only prompts the user to select a route if you’ve configured the audio session with a long-form video route-sharing policy. After the system configures the needed routing, it calls its completion handler, from which you can begin playback.

```
let session = AVAudioSession.sharedInstance()
session.prepareRouteSelectionForPlayback { shouldStartPlayback, routeSelection in
    if shouldStartPlayback {
        // Prepare and present player.
    }
}
```

## See Also

### Related Documentation

func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws

Sets the session category, mode, route-sharing policy, and options.

### Preparing for long-form video playback

enum RouteSelection

Constants used to define the active route selection.

