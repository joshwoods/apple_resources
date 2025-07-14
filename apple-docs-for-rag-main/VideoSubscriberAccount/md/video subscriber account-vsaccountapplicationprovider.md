

- Video Subscriber Account
-  VSAccountApplicationProvider 

Class

# VSAccountApplicationProvider

An object to display app-specific providers in your app.

iOS 14.2+iPadOS 14.2+macOStvOS 14.2+visionOS 1.0+

``` source
class VSAccountApplicationProvider
```

## Overview

The `VSAccountApplicationProvider` object represents an app account provider to be added to the list of already available system TV providers in your app.

## Topics

### Creating an application provider

init(localizedDisplayName: String, identifier: String)

Returns an application provider using a given display name and identifier.

### Application provider details

var identifier: String

A string that identifies a provider.

var localizedDisplayName: String

The display name of the provider as it will appear in the list of providers.

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

### TV app integration

class VSSubscription

An object that describes a subscriber’s access to content.

class VSSubscriptionRegistrationCenter

An object that stores subscription information that the system provides to the Apple TV app.

