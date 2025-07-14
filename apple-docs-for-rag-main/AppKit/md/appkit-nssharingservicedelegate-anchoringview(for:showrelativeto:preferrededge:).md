

- AppKit
- NSSharingServiceDelegate
-  anchoringView(for:showRelativeTo:preferredEdge:) 

Instance Method

# anchoringView(for:showRelativeTo:preferredEdge:)

macOS 10.8+

``` source
@MainActor
optional func anchoringView(
    for sharingService: NSSharingService,
    showRelativeTo positioningRect: UnsafeMutablePointer,
    preferredEdge: UnsafeMutablePointer
) -> NSView?
```

