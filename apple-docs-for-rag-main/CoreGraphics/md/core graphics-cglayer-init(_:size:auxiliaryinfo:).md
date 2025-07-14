

- Core Graphics
- CGLayer
-  init(\_:size:auxiliaryInfo:) 

Initializer

# init(\_:size:auxiliaryInfo:)

Creates a layer object that is associated with a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    _ context: CGContext,
    size: CGSize,
    auxiliaryInfo: CFDictionary?
)
```

## Parameters 

`context`  

The graphics context you want to create the layer relative to. The layer uses this graphics context as a reference for initialization.

`size`  

The size, in default user space units, of the layer relative to the graphics context.

`auxiliaryInfo`  

Reserved for future use. Pass `NULL`.

## Return Value

A CGLayer object. In Objective-C, you’re responsible for releasing this object using the function CGLayerRelease when you no longer need the layer.

## Discussion

After you create a CGLayer object, you should reuse it whenever you can to facilitate the Core Graphics caching strategy. Core Graphics caches any objects that are reused, including CGLayer objects. Objects that are reused frequently remain in the cache. In contrast, objects that are used once in a while may be moved in and out of the cache according to their frequency of use. If you don’t reuse CGLayer objects, Core Graphics won’t cache them. This means that you lose an opportunity to improve the performance of your application.

