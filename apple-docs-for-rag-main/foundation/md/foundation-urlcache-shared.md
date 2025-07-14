

- Foundation
- URLCache
-  shared 

Type Property

# shared

The shared URL cache instance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var shared: URLCache { get set }
```

## Mentioned in 

Accessing cached data

## Discussion

If your app doesn’t have special caching requirements or constraints, the default shared cache instance should be acceptable. Alternatively, you can create a custom URLCache object and set it as the shared cache instance (use `+[NSURLCache setSharedURLCache]` in Objective-C). You should do so before making any calls to this method.

## See Also

### Related Documentation

Accessing cached data

Control how URL requests make use of previously cached data.

