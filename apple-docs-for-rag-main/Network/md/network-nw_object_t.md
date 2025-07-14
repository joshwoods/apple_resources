

- Network
-  nw_object_t 

Type Alias

# nw_object_t

The generic type for objects in the Network framework.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_object_t = any OS_nw_object
```

## Discussion

Network.framework objects are reference-counted objects that can be used with Automatic Reference Counting (ARC) or directly retained and released.

The objects also conform to the description method of NSObject to be used for debugging.

