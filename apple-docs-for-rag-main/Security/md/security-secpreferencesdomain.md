

- Security
-  SecPreferencesDomain 

Enumeration

# SecPreferencesDomain

The keychain preference domains.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecPreferencesDomain
```

## Overview

A preference domain is a set of security-related preferences, such as the default keychain and the current keychain search list. The default preference domain for system daemons (that is, for daemons running in the root session) is the system domain. The default preference domain for all other programs is the user domain. A common preference appears for all users and the system. For example, if you add a keychain to the keychain search list using SecPreferencesDomain.common for the preference domain, the keychain is added to the search list for all users and the system.

## Topics

### Constants

case user

Indicates the user preference domain preferences.

case system

Indicates the system or daemon preference domain preferences.

case common

Indicates the preferences are common to everyone.

case dynamic

Indicates a dynamic search list (typically provided by removable keychains such as smart cards).

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

