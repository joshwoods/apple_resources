

- Foundation
-  URLFileProtection 

Structure

# URLFileProtection

Protection-level values for a URL resource key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLFileProtection
```

## Overview

These are values for the URLResourceKey key fileProtectionKey.

## Topics

### Creating a URL File Protection Type

init(rawValue: String)

### Protection levels

static let complete: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access for reading or writing to while the device is locked or booting.

static let completeUnlessOpen: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk after it closes.

static let completeUntilFirstUserAuthentication: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access until after the device boots.

static let completeWhenUserInactive: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can access only after device unlock and before expiration.

static let none: URLFileProtection

An option that indicates the file has no special protections associated with it.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

struct DirectoryEnumerationOptions

Options for enumerating the contents of directories.

enum SearchPathDirectory

The location of significant directories.

struct SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

struct FileAttributeKey

Keys in dictionaries used to get and set file attributes.

struct FileAttributeType

Values representing a file’s type attribute.

struct FileProtectionType

Protection level values that can be associated with a file attribute key.

