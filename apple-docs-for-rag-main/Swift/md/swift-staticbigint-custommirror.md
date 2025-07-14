

- Swift
- StaticBigInt
-  customMirror 

Instance Property

# customMirror

The custom mirror for this instance.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
var customMirror: Mirror { get }
```

## Discussion

If this type has value semantics, the mirror should be unaffected by subsequent mutations of the instance.

