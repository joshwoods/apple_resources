

- Device Management
- StatusReport
-  StatusReport.Error 

Object

# StatusReport.Error

A status report’s error that contains the status item and the reasons for the error.

Device Assignment ServicesVPP License Management

``` source
object StatusReport.Error
```

## Properties

`Reasons`

`[`StatusReason`]`

An array of reasons for the error.

`StatusItem`

`string`

 (Required) 

The status item that this error pertains to.

## See Also

### Supporting Objects

object StatusReport.StatusItems

The status items for a report.

