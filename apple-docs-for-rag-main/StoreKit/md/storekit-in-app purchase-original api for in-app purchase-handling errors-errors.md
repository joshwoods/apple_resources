

- StoreKit
- In-App Purchase
- Original API for In-App Purchase
-  Handling errors 

Article

# Handling errors

Determine the underlying cause of errors that result from StoreKit requests.

## Overview

A StoreKit request may fail for one of many possible reasons, including invalid product information, invalid payment details, problems with your App Store Connect account, or networking issues. When an error occurs, check the error code to find out what went wrong.

### Determine the cause of the error

When handling errors, such as with the request(_:didFailWithError:) delegate method, it’s important to use the domain and code of the resulting error to determine the underlying cause of failure.

StoreKit uses SKErrorDomain for errors related to payments, store products, and cloud services, as described in SKError.Code. For additional information on troubleshooting StoreKit framework issues, see the In-App Purchase FAQ.

Errors related to networking use NSURLErrorDomain. The following table describes some of the most common networking errors that may occur when using StoreKit:

| Error code | Description |
|----|----|
| NSURLErrorTimedOut (`-1001`) | The connection timed out. |
| NSURLErrorCannotFindHost (`-1003`) | The connection failed because it can’t find the host. |
| NSURLErrorCannotConnectToHost (`-1004`) | The connection failed because it can’t connect to the host. |
| NSURLErrorNetworkConnectionLost (`-1005`) | The connection failed because it lost the network connection. |
| NSURLErrorNotConnectedToInternet (`-1009`) | The connection failed because the device isn’t connected to the internet. |
| NSURLErrorUserCancelledAuthentication (`-1012`) | The connection failed because the user canceled required authentication. |
| NSURLErrorSecureConnectionFailed (`-1200`) | The secure connection failed for an unknown reason. |

## See Also

### Errors

enum Code

Error codes for StoreKit errors.

struct SKError

StoreKit error descriptions, codes, and domains.

let SKErrorDomain: String

The error domain name for StoreKit errors.

