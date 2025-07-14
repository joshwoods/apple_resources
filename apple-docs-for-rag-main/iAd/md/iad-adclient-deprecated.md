

- iAd
-  ADClient Deprecated

Class

# ADClient

The parent class you use to request an attribution response.

``` source
class ADClient
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## Overview

To use this class, fetch the shared client object, shared(). Then call its requestAttributionDetails(_:) method, passing in a block to be called with the result.

## Topics

### Fetching a Shared Client Object

class func shared() -> ADClient

Gets an instance of ADClient.

### Requesting Ad Attribution

func requestAttributionDetails(([String : NSObject]?, (any Error)?) -> Void)

Gets an attribution response.

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

### Essentials

iAd Changelog

Learn what’s new in the Apple Search Ads iAd Attribution API.

Setting Up Apple Search Ads Attribution

Retrieve the attribution dictionary.

