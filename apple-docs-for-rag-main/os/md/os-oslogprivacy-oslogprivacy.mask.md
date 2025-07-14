

- os
- OSLogPrivacy
-  OSLogPrivacy.Mask 

Enumeration

# OSLogPrivacy.Mask

A mask that establishes how the system displays a redacted value in a log message.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum Mask
```

## Topics

### Privacy Mask Options

case hash

An option to replace a redacted value with a string that contains a hashed version of the original value.

case none

An option to replace a redacted value with a generic string.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Creating a Custom Privacy Mask

static func auto(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that determines whether to redact or show values according to their type, and customizes the display of redacted values.

static func `private`(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that marks an interpolated value as private, and customizes the display of redacted values.

static func sensitive(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that marks an interpolated value as sensitive, and customizes the display of redacted values.

