

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  auxiliary 

Type Property

# auxiliary

The behavior marking this window as auxiliary for both Stage Manager and full screen.

macOS 13.0+

``` source
static var auxiliary: NSWindow.CollectionBehavior { get }
```

## Discussion

Marking a window collection behavior as auxiliary means it becomes auxiliary for both Stage Manager and full screen display modes. Auxiliary windows prefer being shown alongside primary windows.

To set a different behavior in full screen, while keeping Stage Manager auxiliary, set a more specific behavior just for full screen mode (see fullScreenNone).

- Swift
- Objective-C

```
window.collectionBehavior = [.auxiliary, .fullScreenNone]
```

```
window.collectionBehavior |= (NSWindowCollectionBehaviorAuxiliary | NSWindowCollectionBehaviorFullScreenNone);
```

Use this collection behavior for About or Settings windows as well as utility panes.

Note

This property is mutually exclusive. Set only one of primary, auxiliary, or canJoinAllApplications on a window handled by Stage Manager at a time.

## See Also

### Stage Manager and full screen

static var primary: NSWindow.CollectionBehavior

The behavior marking this window as primary for both Stage Manager and full screen.

static var canJoinAllApplications: NSWindow.CollectionBehavior

The behavior marking this window as one that can join all apps for both Stage Manager and full screen.

