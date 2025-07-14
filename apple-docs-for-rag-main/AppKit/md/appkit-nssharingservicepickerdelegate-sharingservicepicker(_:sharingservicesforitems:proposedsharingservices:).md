

- AppKit
- NSSharingServicePickerDelegate
-  sharingServicePicker(\_:sharingServicesForItems:proposedSharingServices:) 

Instance Method

# sharingServicePicker(\_:sharingServicesForItems:proposedSharingServices:)

Asks the delegate to specify which services to make available from the sharing service picker.

macOS 10.8+

``` source
optional func sharingServicePicker(
    _ sharingServicePicker: NSSharingServicePicker,
    sharingServicesForItems items: [Any],
    proposedSharingServices proposedServices: [NSSharingService]
) -> [NSSharingService]
```

## Parameters 

`sharingServicePicker`  

The sharing service picker.

`items`  

The items to share. Use the set of items to determine which services are relevant.

`proposedServices`  

The proposed services to include in the sharing service picker.

## Return Value

An array of services to include in the sharing service picker.

## Discussion

Use this method to remove default services, add custom services, or reorder the existing services before the picker appears onscreen. Unless you don’t intend to change the proposed services, create a new mutable array and fill it with the services that are appropriate for the specified set of items. The following example appends a custom NSSharingService object to the proposed list of services.

```
        NSMutableArray *sharingServices = [proposedServices mutableCopy];
        NSSharingService * customService = [[[NSSharingService alloc]   initWithTitle:@"Service Title"
                                                                        image:image alternateImage:alternateImage
                                                                        handler:^{
                                                                            [self doCustomServiceWithItems:items];
                                           }] autorelease];
        [sharingServices addObject:customService];
        return [sharingServices autorelease];
```

