

- AppKit
- NSSharingServiceDelegate
-  sharingService(\_:sourceFrameOnScreenForShareItem:) 

Instance Method

# sharingService(\_:sourceFrameOnScreenForShareItem:)

Invoked when the sharing service is performed and the sharing window is displayed, to present a transition between the original items and the sharing window.

macOS 10.8+

``` source
@MainActor
optional func sharingService(
    _ sharingService: NSSharingService,
    sourceFrameOnScreenForShareItem item: Any
) -> NSRect
```

## Parameters 

`sharingService`  

The sharing service.

`item`  

The item being shared.

## Return Value

The rectangle, in screen coordinates, to display the transition.

## Discussion

The following is an example implementation of this method:

```
- (NSRect)sharingService:(NSSharingService *)sharingService sourceFrameOnScreenForShareItem:(id )item
{
    if ([item isKindOfClass:[NSImage class]]) {
        NSImage * image = [_imageView image];
        NSRect frame = [_imageView bounds];
        frame = [_imageView convertRect:frame toView:nil];
        frame.origin = [[_imageView window] convertBaseToScreen:frame.origin];
        return frame;
    }
    return NSZeroRect;
}
```

## See Also

### Customizing Transition Animation

func sharingService(NSSharingService, transitionImageForShareItem: Any, contentRect: UnsafeMutablePointer&lt;NSRect>) -> NSImage?

Invoked to allow returning a custom transition image when sharing an item.

func sharingService(NSSharingService, sourceWindowForShareItems: [Any], sharingContentScope: UnsafeMutablePointer&lt;NSSharingService.SharingContentScope>) -> NSWindow?

Returns the window that contained the share items.

enum SharingContentScope

The sharing scope constants specify the nature of the things you are sharing.

