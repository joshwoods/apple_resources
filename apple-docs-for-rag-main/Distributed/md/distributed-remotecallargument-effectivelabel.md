

- Distributed
- RemoteCallArgument
-  effectiveLabel 

Instance Property

# effectiveLabel

The effective label of this argument. This reflects the semantics of call sites of function declarations without explicit label definitions in Swift.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var effectiveLabel: String { get }
```

## Discussion

For example, for a method declared like `func hi(a: String)` the effective label is `a` while for a method like `func hi(a b: String)` or `func hi(_ b: String)` the label is the explicitly declared one, so `a` and `_` respectively.

