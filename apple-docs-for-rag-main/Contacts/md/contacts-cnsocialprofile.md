

- Contacts
-  CNSocialProfile 

Class

# CNSocialProfile

An immutable object that represents one of the user’s social profiles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNSocialProfile
```

## Overview

Some social profile services, such as Facebook and Twitter, are predefined in this class. You can also specify your own social profile service with the init(urlString:username:userIdentifier:service:) method.

`CNSocialProfile` objects are thread-safe, and you may access their properties from any thread of your app.

## Topics

### Creating a Social Profile Object

init(urlString: String?, username: String?, userIdentifier: String?, service: String?)

Initializes a new social profile object with the specified URL.

### Getting Social Profile Information

var username: String

The user name for the social profile.

var service: String

The social profile’s service name.

var urlString: String

The URL associated with the social profile.

var userIdentifier: String

The service’s user identifier associated with the social profile.

### Getting Localized User Profile Information

class func localizedString(forKey: String) -> String

Returns the localized name of the property for the specified key.

let CNSocialProfileUsernameKey: String

The social profile user name.

let CNSocialProfileServiceKey: String

The social profile service.

let CNSocialProfileURLStringKey: String

The social profile URL.

let CNSocialProfileUserIdentifierKey: String

The social profile user identifier.

### Getting Localized Service Names

class func localizedString(forService: String) -> String

Returns the localized name of the specified service.

let CNSocialProfileServiceFacebook: String

The Facebook social profile service.

let CNSocialProfileServiceFlickr: String

The Flickr social profile service.

let CNSocialProfileServiceGameCenter: String

The Game Center social profile service.

let CNSocialProfileServiceLinkedIn: String

The LinkedIn social profile service.

let CNSocialProfileServiceMySpace: String

The MySpace social profile service.

let CNSocialProfileServiceSinaWeibo: String

The Sina Weibo social profile service.

let CNSocialProfileServiceTencentWeibo: String

The Tencent Weibo social profile service.

let CNSocialProfileServiceTwitter: String

The Twitter social profile service.

let CNSocialProfileServiceYelp: String

The Yelp social profile service.

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

