

- SwiftUI
- AsyncImage
-  init(url:scale:transaction:content:) 

Initializer

# init(url:scale:transaction:content:)

Loads and displays a modifiable image from the specified URL in phases.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    url: URL?,
    scale: CGFloat = 1,
    transaction: Transaction = Transaction(),
    @ViewBuilder content: @escaping (AsyncImagePhase) -> Content
)
```

## Parameters 

`url`  

The URL of the image to display.

`scale`  

The scale to use for the image. The default is `1`. Set a different value when loading images designed for higher resolution displays. For example, set a value of `2` for an image that you would name with the `@2x` suffix if stored in a file on disk.

`transaction`  

The transaction to use when the phase changes.

`content`  

A closure that takes the load phase as an input, and returns the view to display for the specified phase.

## Discussion

If you set the asynchronous image’s URL to `nil`, or after you set the URL to a value but before the load operation completes, the phase is AsyncImagePhase.empty. After the operation completes, the phase becomes either AsyncImagePhase.failure(_:) or AsyncImagePhase.success(_:). In the first case, the phase’s error value indicates the reason for failure. In the second case, the phase’s image property contains the loaded image. Use the phase to drive the output of the `content` closure, which defines the view’s appearance:

```
AsyncImage(url: URL(string: "https://example.com/icon.png")) { phase in
    if let image = phase.image {
        image // Displays the loaded image.
    } else if phase.error != nil {
        Color.red // Indicates an error.
    } else {
        Color.blue // Acts as a placeholder.
    }
}
```

To add transitions when you change the URL, apply an identifier to the AsyncImage.

