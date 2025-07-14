

- os
- OSLogPrivacy
-  auto(mask:) 

Type Method

# auto(mask:)

Returns a privacy structure that determines whether to redact or show values according to their type, and customizes the display of redacted values.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func auto(mask: OSLogPrivacy.Mask) -> OSLogPrivacy
```

## Parameters 

`mask`  

A mask that determines whether the system replaces a redacted value with a generic string or a string from a hash of the redacted value.

## Return Value

A privacy object that applies the default redaction rules.

## See Also

### Creating a Custom Privacy Mask

static func `private`(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that marks an interpolated value as private, and customizes the display of redacted values.

static func sensitive(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that marks an interpolated value as sensitive, and customizes the display of redacted values.

enum Mask

A mask that establishes how the system displays a redacted value in a log message.

