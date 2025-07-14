

- ManagedSettings
-  Token 

Structure

# Token

A representation of an activity, such as an app or website, that doesn’t reveal its identity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct Token
```

## Overview

Managed Settings uses a `Token` to preserve user privacy and prevent anyone outside of a Family Sharing group from identifying what apps and websites the family accesses. You can use tokens to restrict and filter device use without accessing personal information.

The ManagedSettings framework provides the following types of tokens:

ApplicationToken  
An opaque representation of a selected app.

WebDomainToken  
An opaque representation of a selected web domain.

ActivityCategoryToken  
An opaque representation of a selected category of activity.

## Topics

### Creating a Token

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Encoding a Token

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Comparing Tokens

static func == (Token&lt;T>, Token&lt;T>) -> Bool

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

- Decodable
- Encodable
- Equatable
- Hashable

