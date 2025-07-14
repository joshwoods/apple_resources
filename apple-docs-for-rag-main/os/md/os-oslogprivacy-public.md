

- os
- OSLogPrivacy
-  public 

Type Property

# public

The standard option to always show the interpolated value.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static var `public`: OSLogPrivacy { get }
```

## Mentioned in 

Generating Log Messages from Your Code

## See Also

### Getting the Privacy Options

static var auto: OSLogPrivacy

The standard option to let the system determine whether to redact or display a value.

static var `private`: OSLogPrivacy

The standard option to always redact the interpolated value.

static var sensitive: OSLogPrivacy

The option to always redact interpolated values that contain sensitive information.

