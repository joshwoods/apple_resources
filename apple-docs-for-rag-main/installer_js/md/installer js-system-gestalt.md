

- Installer JS
- System
-  gestalt 

# gestalt

Provides gestalt information that corresponds to the given selector.

``` source
gestalt(selector)
```

## Parameters 

`selector`  

String specifying the selector for the data to retrieve.

## Return Value

Data for the given selector.

## Overview

For example, the expression in Listing 1 returns `'1040'` in OS X v10.4.0:

system.gestalt(&#39;sysv&#39;).toString(16)

See Gestalt Manager for detailed information.

Warning

The underlying Gestalt Manager API is deprecated; use version and sysctl instead of this function.

## See Also

### Legacy Methods

localizedStandardString

Provides the localized standard string in the installation package for the current locale for a given key.

localizedStandardStringWithFormat

Provides the formatted localized standard string in the installation package for the current locale, for a given key and a set of additional arguments.

