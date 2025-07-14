

- Device Management
-  ErrorCodeSoftwareUpdateRequired 

Object

# ErrorCodeSoftwareUpdateRequired

An error response that indicates the system requires a software update.

iOS 17.0+iPadOS 17.0+macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object ErrorCodeSoftwareUpdateRequired
```

## Properties

`code`

`string`

 (Required) 

Indicates that the device needs to perform a software update before enrollment and setup can proceed.

Value: `com.apple.softwareupdate.required`

`description`

`string`

A description of the error. Only use this for logging purposes and don’t display it to the user.

`details`

ErrorCodeSoftwareUpdateRequired.Details

 (Required) 

A description of the error to display to the user.

`message`

`string`

A dictionary that contains additional data about the error code.

## Discussion

The MDM server’s 403 response body contains the schema for a JSON or property list XML document. The response headers need to include a “Content-Type” header that indicates whether the response returns JSON or XML.

The system returns this response when a device attempts to enroll with an MDM server during Setup Assistant, but the MDM server requires the device to perform a software update before it can continue with enrollment and setup.

## Topics

### Details

object ErrorCodeSoftwareUpdateRequired.Details

A dictionary that contains additional data about the software update required error code.

