

- Installer JS
- System
-  localizedStringWithFormat 

# localizedStringWithFormat

Provides the formatted localized string in the installation package for the current locale, for a given key and a set of additional arguments.

``` source
localizedStringWithFormat(stringKey, args...)
```

## Parameters 

`stringKey`  

A string that identifies the desired localized string.

`args...`  

Arguments that replace placeholders (`%@`) in the formatted localized string.

## Return Value

The localized string, if found in the installation package; `null` otherwise.

## See Also

### Internationalizing Distributions

localizedString

Provides the localized string in the installation package for the current locale for a given key.

