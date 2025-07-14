

- Create ML
- MLDataColumn
-  customMirror 

Instance Property

# customMirror

The custom mirror for this instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var customMirror: Mirror { get }
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Discussion

If this type has value semantics, the mirror should be unaffected by subsequent mutations of the instance.

