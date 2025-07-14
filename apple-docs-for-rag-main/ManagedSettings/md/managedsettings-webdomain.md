

- ManagedSettings
-  WebDomain 

Structure

# WebDomain

An object that represents a website.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct WebDomain
```

## Topics

### Creating a Web Domain

init(domain: String)

Creates an object that represents the specified web domain.

init(token: WebDomainToken)

Creates an object that represents the provided domain.

### Identifying a Web Domain

let domain: String?

A string that identifies a specific web domain.

let token: WebDomainToken?

An opaque representation of a specific web domain.

### Comparing Web Domains

static func == (WebDomain, WebDomain) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Websites

typealias WebDomainToken

A representation of a web domain that preserves the user’s privacy.

