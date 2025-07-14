

- AppKit
- NSWindow
- NSWindow.CollectionBehavior
-  primary 

Type Property

# primary

The behavior marking this window as primary for both Stage Manager and full screen.

macOS 13.0+

``` source
static var primary: NSWindow.CollectionBehavior { get }
```

## Discussion

Marking a window collection behavior as primary means it becomes primary for both Stage Manager and full screen display modes.

To set a different behavior in full screen while keeping Stage Manager primary, set a more specific behavior just for full screen mode (see fullScreenAuxiliary).

- Swift
- Objective-C

```
window.collectionBehavior = [.primary, .fullScreenAuxiliary]
```

```
window.collectionBehavior |= (NSWindowCollectionBehaviorPrimary | NSWindowCollectionBehaviorFullScreenAuxiliary);
```

Use this collection behavior for document or viewer windows.

Note

This property is mutually exclusive. Set only one of primary, auxiliary, or canJoinAllApplications on a window handled by Stage Manager at a time.

## See Also

### Stage Manager and full screen

static var auxiliary: NSWindow.CollectionBehavior

The behavior marking this window as auxiliary for both Stage Manager and full screen.

static var canJoinAllApplications: NSWindow.CollectionBehavior

The behavior marking this window as one that can join all apps for both Stage Manager and full screen.

