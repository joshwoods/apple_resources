

- AppKit
- NSSharingServiceDelegate
-  sharingService(\_:sourceWindowForShareItems:sharingContentScope:) 

Instance Method

# sharingService(\_:sourceWindowForShareItems:sharingContentScope:)

Returns the window that contained the share items.

macOS 10.8+

``` source
@MainActor
optional func sharingService(
    _ sharingService: NSSharingService,
    sourceWindowForShareItems items: [Any],
    sharingContentScope: UnsafeMutablePointer
) -> NSWindow?
```

## Parameters 

`sharingService`  

The sharing service.

`items`  

The items being shared.

`sharingContentScope`  

The sharing content scope. The sharing scope can be modified from the default value of NSSharingService.SharingContentScope.item by setting a different value in the out parameter `sharingContentScope`. See NSSharingService.SharingContentScope for supported values.

## Return Value

The window of the shared items.

## Discussion

The following is an example implementation of this method. It changes the item scope, and returns the window the source image view is contained within.

```
- (NSWindow *)sharingService:(NSSharingService *)sharingService
              sourceWindowForShareItems:(NSArray *)items
              sharingContentScope:(NSSharingContentScope *)sharingContentScope
{
    *sharingContentScope = NSSharingContentScopeItem;
    return [_imageView window];
}
```

## See Also

### Customizing Transition Animation

func sharingService(NSSharingService, sourceFrameOnScreenForShareItem: Any) -> NSRect

Invoked when the sharing service is performed and the sharing window is displayed, to present a transition between the original items and the sharing window.

func sharingService(NSSharingService, transitionImageForShareItem: Any, contentRect: UnsafeMutablePointer&lt;NSRect>) -> NSImage?

Invoked to allow returning a custom transition image when sharing an item.

enum SharingContentScope

The sharing scope constants specify the nature of the things you are sharing.

