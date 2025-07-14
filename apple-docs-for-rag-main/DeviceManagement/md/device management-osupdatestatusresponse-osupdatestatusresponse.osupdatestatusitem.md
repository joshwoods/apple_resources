

- Device Management
- OSUpdateStatusResponse
-  OSUpdateStatusResponse.OSUpdateStatusItem 

Device Management Command

# OSUpdateStatusResponse.OSUpdateStatusItem

A dictionary that describes the status of a software update.

iOS 9.0+iPadOS 9.0+macOS 10.11.5+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object OSUpdateStatusResponse.OSUpdateStatusItem
```

## Properties

`DeferralsRemaining`

`integer`

The number of remaining user deferrals for this OS update.

Available in macOS 12.3 and later.

`DownloadPercentComplete`

`number`

 (Required) 

A floating-point number between `0.0` and `1.0` that indicates the download progress as a percentage.

`IsDownloaded`

`boolean`

 (Required) 

If `true`, the update has finished downloading.

`MaxDeferrals`

`integer`

The number of times a user can defer this OS update.

Available in macOS 12.3 and later.

`NextScheduledInstall`

`date`

The date of the next attempt at installing this OS update.

Available in macOS 12.3 and later.

`PastNotifications`

`[date]`

The dates/times when the OS notified the user about installing this OS update.

Available in macOS 12.3 and later.

`ProductKey`

`string`

 (Required) 

The product key that represents the update.

`Status`

`string`

 (Required) 

The status of the update, which is one of the following values:

- `Idle`: The update is idle.

- `Downloading`: The software update is downloading and subsequently preparing.

- `Installing`: The software update is installing.

## See Also

### Commands

object OSUpdateStatusResponse.ErrorChainItem

A dictionary that describes an error chain item.

