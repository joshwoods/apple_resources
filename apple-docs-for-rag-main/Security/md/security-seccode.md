

- Security
-  SecCode 

Class

# SecCode

A code object representing signed code running on the system.

Mac Catalyst 13.0+macOS 10.0+

``` source
class SecCode
```

## Mentioned in 

Hosting Guest Code

## Overview

In many function calls, a value of type SecCode can be passed to a parameter that is typed as a SecStaticCode. In these cases, the function performs an implicit call to the SecCodeCopyStaticCode(_:_:_:) function and operates on the result.

## Relationships

### Conforms To

- Equatable
- Hashable

