

- AppKit
- NSButtonTouchBarItem
-  init(identifier:title:image:target:action:) 

Initializer

# init(identifier:title:image:target:action:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

**macOS**

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    title: String,
    image: NSImage,
    target: Any?,
    action: Selector?
)
```

**Mac Catalyst**

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    title: String,
    image: UIImage,
    target: Any?,
    action: Selector?
)
```

## See Also

### Creating a button item

convenience init(identifier: NSTouchBarItem.Identifier, image: UIImage, target: Any?, action: Selector?)

convenience init(identifier: NSTouchBarItem.Identifier, title: String, target: Any?, action: Selector?)

