

- PHASE
- PHASEMetaParameter
-  value 

Instance Property

# value

A value for the metaparameter.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var value: Any { get set }
```

## Discussion

The framework sets this property to the subclass’s initializer argument; for example, see init(value:).

An app changes the value at runtime by calling fade(value:duration:) on the subclass.

