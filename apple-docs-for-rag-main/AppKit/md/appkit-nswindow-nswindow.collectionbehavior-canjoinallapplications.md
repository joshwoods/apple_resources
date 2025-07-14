

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  canJoinAllApplications 

Type Property

# canJoinAllApplications

The behavior marking this window as one that can join all apps for both Stage Manager and full screen.

macOS 13.0+

``` source
static var canJoinAllApplications: NSWindow.CollectionBehavior { get }
```

## Discussion

Windows marked with this behavior don’t participate in Stage Manager layout but can join the windows of other apps in full screen spaces when eligible.

Use this collection behavior for floating windows and system overlays. To opt out of joining other apps’ full screen spaces use fullScreenPrimary.

Note

This property is mutually exclusive. Set only one of primary, auxiliary, or canJoinAllApplications on a window handled by Stage Manager at a time.

## See Also

### Stage Manager and full screen

static var primary: NSWindow.CollectionBehavior

The behavior marking this window as primary for both Stage Manager and full screen.

static var auxiliary: NSWindow.CollectionBehavior

The behavior marking this window as auxiliary for both Stage Manager and full screen.

