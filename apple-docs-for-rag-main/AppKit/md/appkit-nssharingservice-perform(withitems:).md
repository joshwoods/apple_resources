

- AppKit
- NSSharingService
-  perform(withItems:) 

Instance Method

# perform(withItems:)

Manually performs the service on the provided items.

macOS 10.8+

``` source
func perform(withItems items: [Any])
```

## Parameters 

`items`  

The items to share.

## Discussion

In most cases this will display a sharing window.

## See Also

### Related Documentation

func canPerform(withItems: [Any]?) -> Bool

Returns whether the service can share all the specified items.

