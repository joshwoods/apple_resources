

- UIKit
- UIView
-  tag 

Instance Property

# tag

An integer that you can use to identify view objects in your application.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tag: Int { get set }
```

## Discussion

The default value is `0`. You can set the value of this tag and use that value to identify the view later.

## See Also

### Identifying the view at runtime

func viewWithTag(Int) -> UIView?

Returns the view whose tag matches the specified value.

