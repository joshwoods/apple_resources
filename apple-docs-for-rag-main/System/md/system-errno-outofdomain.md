

- System
- Errno
-  outOfDomain 

Type Property

# outOfDomain

Numerical argument out of domain.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var outOfDomain: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A numerical input argument was outside the defined domain of the mathematical function.

The corresponding C error is `EDOM`.

## See Also

### Math Errors

static var outOfRange: Errno

Numerical result out of range.

static var overflow: Errno

Value too large to be stored in data type.

