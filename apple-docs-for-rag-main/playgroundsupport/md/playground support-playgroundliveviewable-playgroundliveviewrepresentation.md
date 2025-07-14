

- Playground Support
- PlaygroundLiveViewable
-  playgroundLiveViewRepresentation 

Instance Property

# playgroundLiveViewRepresentation

The view or view controller used to render and manage the live view.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

``` source
var playgroundLiveViewRepresentation: PlaygroundLiveViewRepresentation { get }
```

**Required**

## Return Value

A view or view controller able to render and manage the live view. View controllers are preferred.

Important

The view or view controller returned by this method must be the root of the hierarchy. Views can't have superviews or associated view controllers, and view controllers can't have parent view controllers.

## Discussion

The value returned by `playgroundLiveViewRepresentation` can be different each time the property is accessed.

