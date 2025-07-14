

- System
- Errno
-  lastErrnoValue 

Type Property

# lastErrnoValue

The largest valid error.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var lastErrnoValue: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

This value is the largest valid value encountered using the C `errno` global variable. It isn’t a valid error.

The corresponding C error is `ELAST`.

## See Also

### Reserved

static var multiHop: Errno

Reserved.

static var noLink: Errno

Reserved.

static var noStreamResources: Errno

Reserved.

static var notStream: Errno

Reserved.

static var notUsed: Errno

Error. Not used.

static var timeout: Errno

Reserved.

