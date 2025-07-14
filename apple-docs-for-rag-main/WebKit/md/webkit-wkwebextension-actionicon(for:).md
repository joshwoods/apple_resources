

- WebKit
- WKWebExtension
-  actionIcon(for:) 

Instance Method

# actionIcon(for:)

Returns the default action icon for the specified size.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

**macOS**

``` source
@MainActor
func actionIcon(for size: CGSize) -> NSImage?
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
func actionIcon(for size: CGSize) -> UIImage?
```

## Parameters 

`size`  

The size to use when looking up the action icon.

## Return Value

The action icon, or `nil` if the icon was unable to be loaded.

## Discussion

This icon serves as a default and should be used to represent the extension in contexts like action sheets or toolbars prior to the extension being loaded into an extension context. Once the extension is loaded, use the action(for:) API to get the tab-specific icon.

The returned image will be the best match for the specified size that is available in the extension’s action icon set. If no matching icon is available, the method will fall back to the extension’s icon.

## See Also

### Related Documentation

func icon(for: CGSize) -> UIImage?

Returns the extension’s icon image for the specified size.

