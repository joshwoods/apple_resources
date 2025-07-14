

- AppKit
- NSSharingService
-  sharingServices(forItems:) Deprecated

Type Method

# sharingServices(forItems:)

Returns a list of sharing services which could share all the provided items together.

macOS 10.8–13.0Deprecated

``` source
class func sharingServices(forItems items: [Any]) -> [NSSharingService]
```

Deprecated

Use -\[NSSharingServicePicker standardShareMenuItem\] instead.

## Parameters 

`items`  

The items to share.

## Return Value

An array of sharing services to allow for `items`.

## Discussion

This method can be used to build a custom user interface or to populate a contextual menu.

## See Also

### Related Documentation

init?(named: NSSharingService.Name)

Returns a sharing service instance representing the specified service name.

### Querying Service Availability

func canPerform(withItems: [Any]?) -> Bool

Returns whether the service can share all the specified items.

