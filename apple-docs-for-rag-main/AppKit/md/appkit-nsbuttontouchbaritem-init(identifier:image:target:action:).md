

- AppKit
- NSButtonTouchBarItem
-  init(identifier:image:target:action:) 

Initializer

# init(identifier:image:target:action:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

**Mac Catalyst**

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    image: UIImage,
    target: Any?,
    action: Selector?
)
```

**macOS**

``` source
@MainActor
convenience init(
    identifier: NSTouchBarItem.Identifier,
    image: NSImage,
    target: Any?,
    action: Selector?
)
```

## See Also

### Creating a button item

convenience init(identifier: NSTouchBarItem.Identifier, title: String, image: UIImage, target: Any?, action: Selector?)

convenience init(identifier: NSTouchBarItem.Identifier, title: String, target: Any?, action: Selector?)

