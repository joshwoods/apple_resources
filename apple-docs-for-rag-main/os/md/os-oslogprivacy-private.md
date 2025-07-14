

- os
- OSLogPrivacy
-  private 

Type Property

# private

The standard option to always redact the interpolated value.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static var `private`: OSLogPrivacy { get }
```

## Mentioned in 

Generating Log Messages from Your Code

## Discussion

When it redacts a value, the system displays a generic string in place of the value. If you want to correlate log messages that contain the same value, use the private(mask:) function to create a structure with the OSLogPrivacy.Mask.hash mask.

## See Also

### Getting the Privacy Options

static var auto: OSLogPrivacy

The standard option to let the system determine whether to redact or display a value.

static var `public`: OSLogPrivacy

The standard option to always show the interpolated value.

static var sensitive: OSLogPrivacy

The option to always redact interpolated values that contain sensitive information.

