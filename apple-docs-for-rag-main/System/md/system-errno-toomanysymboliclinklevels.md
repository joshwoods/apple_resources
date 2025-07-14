

- System
- Errno
-  tooManySymbolicLinkLevels 

Type Property

# tooManySymbolicLinkLevels

Too many levels of symbolic links.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var tooManySymbolicLinkLevels: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A pathname lookup involved more than eight symbolic links.

The corresponding C error is `ELOOP`.

## See Also

### Path Errors

static var fileNameTooLong: Errno

The file name is too long.

static var tooManyRemoteLevels: Errno

Too many levels of remote in path.

