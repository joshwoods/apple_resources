

- Distributed
- RemoteCallArgument
-  label 

Instance Property

# label

The “argument label” of the argument. The label is the name visible name used in external calls made to this target, e.g. for `func hello(label name: String)` it is `label`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
let label: String?
```

## Discussion

If no label is specified (i.e. `func hi(name: String)`), the `label`, value is empty, however `effectiveLabel` is equal to the `name`.

In most situations, using `effectiveLabel` is more useful to identify the user-visible name of this argument.

