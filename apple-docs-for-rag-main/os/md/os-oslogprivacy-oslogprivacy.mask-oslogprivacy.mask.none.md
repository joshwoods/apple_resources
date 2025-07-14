

- os
- OSLogPrivacy
- OSLogPrivacy.Mask
-  OSLogPrivacy.Mask.none 

Case

# OSLogPrivacy.Mask.none

An option to replace a redacted value with a generic string.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case none
```

## Discussion

Use this option when you don’t want to correlate log messages with identical redacted values.

## See Also

### Privacy Mask Options

case hash

An option to replace a redacted value with a string that contains a hashed version of the original value.

