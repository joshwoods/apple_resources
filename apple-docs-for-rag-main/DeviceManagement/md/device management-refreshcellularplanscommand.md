

- Device Management
-  RefreshCellularPlansCommand 

Device Management Command

# RefreshCellularPlansCommand

The command to query a carrier URL for active eSIM cellular-plan profiles.

iOS 13.0+iPadOS 13.0+Device Assignment ServicesVPP License Management

``` source
object RefreshCellularPlansCommand
```

## Properties

`Command`

RefreshCellularPlansCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object RefreshCellularPlansCommand.Command

The request dictionary to query a carrier URL for active eSIM cellular-plan profiles.

## See Also

### Command and Response

object RefreshCellularPlansResponse

A response from the device after it processes the command to query a carrier URL for active eSIM cellular-plan profiles.

