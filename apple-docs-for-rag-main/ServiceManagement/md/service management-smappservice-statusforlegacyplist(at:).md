

- Service Management
- SMAppService
-  statusForLegacyPlist(at:) 

Type Method

# statusForLegacyPlist(at:)

Check the authorization status of an earlier OS version login item.

Mac Catalyst 16.0+macOS 13.0+

``` source
class func statusForLegacyPlist(at url: URL) -> SMAppService.Status
```

## Parameters 

`url`  

The URL of the helper executable’s property list.

## Return Value

One of the SMAppService.Status constants that indicate the current authorization status.

## Mentioned in 

Updating helper executables from earlier versions of macOS

