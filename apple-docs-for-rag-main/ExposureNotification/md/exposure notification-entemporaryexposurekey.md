

- Exposure Notification
-  ENTemporaryExposureKey 

Class

# ENTemporaryExposureKey

The key used to generate rolling proximity identifiers.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
class ENTemporaryExposureKey
```

## Overview

Important

This class is available in iOS 12.5, and in iOS 13.5 and later.

Upon a positive diagnosis, the user is allowed to submit their temporary exposure keys to their Health Authority server as diagnosis keys. Use getDiagnosisKeys(completionHandler:) to obtain the user’s diagnosis keys for submission.

## Topics

### Exposure Criteria

var transmissionRiskLevel: ENRiskLevel

The risk of transmission associated with the person a key came from.

var rollingPeriod: ENIntervalNumber

The length of time that this key is valid.

var keyData: Data

The temporary exposure key information.

var rollingStartNumber: ENIntervalNumber

A number that indicates when a key’s rolling period started.

typealias ENIntervalNumber

A number assigned to each 10-minute window shared between all devices participating in the protocol.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Obtaining Exposure Keys

func getDiagnosisKeys(completionHandler: ENGetDiagnosisKeysHandler)

Requests the temporary exposure keys from the user’s device to share with a server.

func getTestDiagnosisKeys(completionHandler: ENGetDiagnosisKeysHandler)

Requests the temporary exposure keys, including the current key, used by this device for testing.

