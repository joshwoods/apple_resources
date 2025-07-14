

- Security
-  errSecCSSigDBDenied 

Global Variable

# errSecCSSigDBDenied

Access to signature database denied.

Mac Catalyst 13.0+macOS 10.0+

``` source
var errSecCSSigDBDenied: OSStatus { get }
```

## Discussion

This error is returned when the system is attempting to sign unsigned code ad-hoc and couldn’t write to the signature database because of a permission problem.

