

- Foundation
-  NSItemProviderPreferredImageSizeKey 

Global Variable

# NSItemProviderPreferredImageSizeKey

A key provided to the options dictionary to indicate a preferred image size.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSItemProviderPreferredImageSizeKey: String
```

## Discussion

Use this key only with the NSItemProvider type coercion policy. Ensure the value is an NSValue object that contains a CGSize struct specifying the requested size, in points.

