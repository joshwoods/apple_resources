

- AppKit
- NSTreeController
-  content 

Instance Property

# content

The tree controller’s content object.

macOS

``` source
var content: Any? { get set }
```

## Discussion

The value of this property can be an array of objects, or a single root object. The default value is `nil`. This property is observable using key-value observing.

