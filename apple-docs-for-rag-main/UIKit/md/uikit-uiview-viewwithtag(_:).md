

- UIKit
- UIView
-  viewWithTag(\_:) 

Instance Method

# viewWithTag(\_:)

Returns the view whose tag matches the specified value.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func viewWithTag(_ tag: Int) -> UIView?
```

## Parameters 

`tag`  

The tag value to search for.

## Return Value

The view in the receiver’s hierarchy whose tag property matches the value in the `tag` parameter.

## Discussion

This method searches the current view and all of its subviews for the specified view.

## See Also

### Identifying the view at runtime

var tag: Int

An integer that you can use to identify view objects in your application.

