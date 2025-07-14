

- ProximityReader
- MobileDocumentReaderError
-  MobileDocumentReaderError.sessionExpired 

Case

# MobileDocumentReaderError.sessionExpired

An error that indicates the current reader session has expired.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
case sessionExpired
```

## Mentioned in 

Adopting the Verifier API in your iPhone app

## Discussion

Generate a new reader token and call prepare(using:) again.

## See Also

### Getting the error code

case cancelled

An error that indicates the mobile document request was canceled.

case invalidRequest

An error that indicates the request isn’t valid.

case invalidResponse

An error that indicates the response isn’t valid.

case invalidToken

An error that indicates the provided reader token for framework’s prepare method isn’t valid.

case networkUnavailable

An error that indicates the system can’t reach the network.

case notAllowed

An error that indicates the device isn’t allowed to perform the mobile document request.

case notSupported

An error that indicates mobile document reading isn’t supported on the current device.

case serviceUnavailable

An error that occurs when mobile document reader service is unavailable.

case systemBusy

An error that indicates the system is busy.

case unknown

An error that indicates the framework encountered a problem which the system can’t interpret.

