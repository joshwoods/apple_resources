

- Foundation
- URLSessionConfiguration
-  backgroundSessionConfiguration(\_:) Deprecated

Type Method

# backgroundSessionConfiguration(\_:)

Returns a session configuration object that allows HTTP and HTTPS uploads or downloads to be performed in the background.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class func backgroundSessionConfiguration(_ identifier: String) -> URLSessionConfiguration
```

Deprecated

Use background(withIdentifier:) instead.

## Parameters 

`identifier`  

The unique identifier for the configuration object. This parameter must not be `nil` or an empty string.

## Return Value

A URL session configuration object that causes upload and download tasks to be performed by the system in a separate process.

