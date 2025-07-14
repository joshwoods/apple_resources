

- System
- Errno
-  outOfRange 

Type Property

# outOfRange

Numerical result out of range.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var outOfRange: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A numerical result of the function was too large to fit in the available space; for example, because it exceeded a floating point number’s level of precision.

The corresponding C error is `ERANGE`.

## See Also

### Math Errors

static var outOfDomain: Errno

Numerical argument out of domain.

static var overflow: Errno

Value too large to be stored in data type.

