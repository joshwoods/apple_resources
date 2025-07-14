

- ProximityReader
-  MobileDocumentReaderError 

Enumeration

# MobileDocumentReaderError

An error type that indicates problems when preparing a mobile document reader session and performing document requests.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum MobileDocumentReaderError
```

## Mentioned in 

Adopting the Verifier API in your iPhone app

## Topics

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

case sessionExpired

An error that indicates the current reader session has expired.

case systemBusy

An error that indicates the system is busy.

case unknown

An error that indicates the framework encountered a problem which the system can’t interpret.

### Operators

static func == (MobileDocumentReaderError, MobileDocumentReaderError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var errorDescription: String?

A localized message describing what error occurred.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

## See Also

### Errors

enum PaymentCardReaderError

An error type that indicates problems with the configuration of the reader.

