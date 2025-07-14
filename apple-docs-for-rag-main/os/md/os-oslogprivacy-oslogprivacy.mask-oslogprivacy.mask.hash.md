

- os
- OSLogPrivacy
- OSLogPrivacy.Mask
-  OSLogPrivacy.Mask.hash 

Case

# OSLogPrivacy.Mask.hash

An option to replace a redacted value with a string that contains a hashed version of the original value.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case hash
```

## Mentioned in 

Generating Log Messages from Your Code

## Discussion

Use this option when you want to hide potentially sensitive data in log messages, but still want to know when two or more log messages contain the same hidden value. An OSLogPrivacy structure with this option generates a hash string for a redacted value. The system displays that hash string as part of the log message, making it possible for you to compare log messages with the same value.

## See Also

### Privacy Mask Options

case none

An option to replace a redacted value with a generic string.

