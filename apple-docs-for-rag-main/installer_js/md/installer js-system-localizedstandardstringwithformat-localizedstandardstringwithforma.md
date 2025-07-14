

- Installer JS
- System
-  localizedStandardStringWithFormat 

# localizedStandardStringWithFormat

Provides the formatted localized standard string in the installation package for the current locale, for a given key and a set of additional arguments.

``` source
localizedStandardStringWithFormat(stringKey, args...)
```

## Parameters 

`stringKey`  

A string that identifies the desired localized string.

`args...`  

Arguments that replace placeholders (`%@`) in the formatted localized string.

## Return Value

The localized string, if found in the installation package; `null` otherwise.

## Overview

This method is not supported. Use localizedStringWithFormat instead.

## See Also

### Legacy Methods

gestalt

Provides gestalt information that corresponds to the given selector.

localizedStandardString

Provides the localized standard string in the installation package for the current locale for a given key.

