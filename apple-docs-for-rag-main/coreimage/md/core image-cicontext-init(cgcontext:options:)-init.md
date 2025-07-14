

- Core Image
- CIContext
-  init(cgContext:options:) 

Initializer

# init(cgContext:options:)

Creates a Core Image context from a Quartz context, using the specified options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(
    cgContext cgctx: CGContext,
    options: [CIContextOption : Any]? = nil
)
```

## Parameters 

`ctx`  

A Quartz graphics context (CGContext object) either obtained from the system or created using a Quartz function such as init(data:width:height:bitsPerComponent:bytesPerRow:space:bitmapInfo:). See Quartz 2D Programming Guide for information on creating Quartz graphics contexts.

`dict`  

A dictionary that contains color space information. You can pass any of the keys defined in `Context Options` along with the appropriate value.

## Discussion

After calling this method, Core Image draws content to the specified Quartz graphics context.

When you create a `CIContext` object using a Quartz graphics context, any transformations that are already set on the Quartz graphics context affect drawing to that context.

Note

To obtain a Core Image context for the current AppKit drawing context in macOS, use the NSGraphicsContext ciContext property.

