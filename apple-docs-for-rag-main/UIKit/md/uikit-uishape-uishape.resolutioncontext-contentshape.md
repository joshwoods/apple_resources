

- UIKit
- UIShape
- UIShape.ResolutionContext
-  contentShape 

Instance Property

# contentShape

The resolved shape of the content to which this shape can apply.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
var contentShape: UIShape.Resolved
```

## Discussion

For example, if this shape applies an effect to a button, the contentShape might represent the bounding shape of that button’s background. You typically size a dynamic shape relative to the bounding rectangle of the contentShape.

