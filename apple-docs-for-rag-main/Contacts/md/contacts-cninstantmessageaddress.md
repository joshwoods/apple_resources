

- Contacts
-  CNInstantMessageAddress 

Class

# CNInstantMessageAddress

An immutable object representing an instant message address for the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNInstantMessageAddress
```

## Overview

Use the methods and properties of `CNInstantMessageAddress` to identify instant messaging addresses. Some instant message services, such as Facebook and Skype are predefined in this class. You can also specify your own instant message service using the init(username:service:) method.

`CNInstantMessageAddress` objects are thread-safe, and you may access their properties from any thread of your app.

## Topics

### Creating an Instant Message Address

init(username: String, service: String)

Returns a CNInstantMessageAddress object initialized with the specified user name and service.

### Getting the Address Information

var service: String

The name of the instant message address service.

var username: String

The user name for instant message service address.

### Getting Localized Address Information

class func localizedString(forKey: String) -> String

Returns a string containing the localized property name.

let CNInstantMessageAddressUsernameKey: String

Instant message address username key.

let CNInstantMessageAddressServiceKey: String

Instant message address service key.

### Getting Localized Service Names

class func localizedString(forService: String) -> String

Returns a string containing the localized name of the specified service.

let CNInstantMessageServiceAIM: String

Instant message service for AIM.

let CNInstantMessageServiceFacebook: String

Instant message service for Facebook.

let CNInstantMessageServiceGaduGadu: String

Instant message service for Gadu Gadu.

let CNInstantMessageServiceGoogleTalk: String

Instant message service for Google Talk.

let CNInstantMessageServiceICQ: String

Instant message service for ICQ.

let CNInstantMessageServiceJabber: String

Instant message service for Jabber.

let CNInstantMessageServiceMSN: String

Instant message service for MSN.

let CNInstantMessageServiceQQ: String

Instant message service for QQ.

let CNInstantMessageServiceSkype: String

Instant message service for Skype.

let CNInstantMessageServiceYahoo: String

Instant message service for Yahoo.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Addresses

class CNPostalAddress

An immutable representation of the postal address for a contact.

class CNMutablePostalAddress

A mutable representation of the postal address for a contact.

