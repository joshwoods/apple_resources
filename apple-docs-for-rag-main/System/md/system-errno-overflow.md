

- System
- Errno
-  overflow 

Type Property

# overflow

Value too large to be stored in data type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var overflow: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A numerical result of the function is too large to be stored in the space that the caller provided.

The corresponding C error is `EOVERFLOW`.

## See Also

### Math Errors

static var outOfDomain: Errno

Numerical argument out of domain.

static var outOfRange: Errno

Numerical result out of range.

