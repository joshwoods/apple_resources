

- AppKit
- NSSharingServiceDelegate
-  sharingService(\_:transitionImageForShareItem:contentRect:) 

Instance Method

# sharingService(\_:transitionImageForShareItem:contentRect:)

Invoked to allow returning a custom transition image when sharing an item.

macOS 10.8+

``` source
@MainActor
optional func sharingService(
    _ sharingService: NSSharingService,
    transitionImageForShareItem item: Any,
    contentRect: UnsafeMutablePointer
) -> NSImage?
```

## Parameters 

`sharingService`  

The sharing service.

`item`  

The shared item.

`contentRect`  

The content rectangle is the frame of the actual content inside the transition image, excluding all decorations. For example, if the transition image is a QuickLook thumbnail, the value would be `QLThumbnailGetContentRect`.

## Return Value

The image to display for the sharing transition. Its size should exactly match that of the original image.

## Discussion

A sample implementation of this method:

```
- (NSImage *)sharingService:(NSSharingService *)sharingService
             transitionImageForShareItem:(id )item
             contentRect:(NSRect *)contentRect
{
    if ([item isKindOfClass:[NSImage class]]) {
        return [_imageView image];
    }
}
```

## See Also

### Customizing Transition Animation

func sharingService(NSSharingService, sourceFrameOnScreenForShareItem: Any) -> NSRect

Invoked when the sharing service is performed and the sharing window is displayed, to present a transition between the original items and the sharing window.

func sharingService(NSSharingService, sourceWindowForShareItems: [Any], sharingContentScope: UnsafeMutablePointer&lt;NSSharingService.SharingContentScope>) -> NSWindow?

Returns the window that contained the share items.

enum SharingContentScope

The sharing scope constants specify the nature of the things you are sharing.

