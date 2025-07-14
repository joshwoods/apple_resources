

- Core NFC
-  VASErrorCode Deprecated

Type Alias

# VASErrorCode

Constants representing APDU status codes for a VAS response.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
typealias VASErrorCode = NFCVASResponse.ErrorCode
```

## Topics

### Status Codes

static var VASErrorCodeSuccess: NFCVASResponse.ErrorCode

A constant indicating that the `GET VAS DATA` command was successful.

static var VASErrorCodeUserIntervention: NFCVASResponse.ErrorCode

A constant indicating that the tag requires user intervention.

### Data Codes

static var VASErrorCodeDataNotActivated: NFCVASResponse.ErrorCode

A constant indicating that the data isn’t activated.

static var VASErrorCodeDataNotFound: NFCVASResponse.ErrorCode

A constant indicating that data wasn’t found.

static var VASErrorCodeIncorrectData: NFCVASResponse.ErrorCode

A constant indicating that the data is incorrect.

### Error Codes

static var VASErrorCodeUnsupportedApplicationVersion: NFCVASResponse.ErrorCode

A constant indicating an unsupported application version.

static var VASErrorCodeWrongLCField: NFCVASResponse.ErrorCode

A constant indicating that the value in the Length Count field is wrong.

static var VASErrorCodeWrongParameters: NFCVASResponse.ErrorCode

A constant indicating that VAS command parameters are wrong.

## See Also

### Getting the Response Status

var status: NFCVASResponse.ErrorCode

A response APDU status code.

