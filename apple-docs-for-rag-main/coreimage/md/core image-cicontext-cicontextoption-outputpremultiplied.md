

- Core Image
- CIContext
- CIContextOption
-  outputPremultiplied 

Type Property

# outputPremultiplied

An option for whether output rendering by the context produces alpha-premultiplied pixels.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
static let outputPremultiplied: CIContextOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value of `true` produces premultiplied output.

