

- AppKit
- NSDictionaryController
-  localizedKeyDictionary 

Instance Property

# localizedKeyDictionary

The localized key names that are displayed by the receiver in place of the key names.

macOS 10.5+

``` source
var localizedKeyDictionary: [String : String] { get set }
```

## Discussion

The dictionary contains the key names as the keys, and the localized key names as the corresponding values.

## See Also

### Localizing Key Names

var localizedKeyTable: String?

the strings file used to localize key names.

