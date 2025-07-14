

- AppKit
- NSSharingService
-  canPerform(withItems:) 

Instance Method

# canPerform(withItems:)

Returns whether the service can share all the specified items.

macOS 10.8+

``` source
func canPerform(withItems items: [Any]?) -> Bool
```

## Parameters 

`items`  

The items to share.

## Return Value

true if the service can share all the items; false otherwise. If `items` is `nil`, the method will return true when the service is configured.

## Discussion

This method can be used to validate a custom user interface such as a dedicated Twitter button. Therefore you could call it once at launch time with `nil` items to check whether to display the button or not, and then with real items to enable and disable the button depending on the context or selection.

## See Also

### Related Documentation

func perform(withItems: [Any])

Manually performs the service on the provided items.

### Querying Service Availability

class func sharingServices(forItems: [Any]) -> [NSSharingService]

Returns a list of sharing services which could share all the provided items together.

Deprecated

