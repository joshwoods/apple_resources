

- AppKit
-  NSCloudSharingValidation 

Protocol

# NSCloudSharingValidation

A protocol that a Cloud-sharing toolbar item uses to get validation of an item.

macOS

``` source
protocol NSCloudSharingValidation : NSObjectProtocol
```

## Topics

### Getting an item’s Cloud share

func cloudShare(for: any NSValidatedUserInterfaceItem) -> CKShare?

Returns the Cloud share object that corresponds to the specified item, if one exists.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

