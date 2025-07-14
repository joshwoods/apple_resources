

- AppKit
- NSTextAlternatives
-  selectedAlternativeStringNotification 

Type Property

# selectedAlternativeStringNotification

Posted when the user selects an alternate string.

macOS 10.8+

``` source
class let selectedAlternativeStringNotification: NSNotification.Name
```

## Discussion

Arbitrary objects can listen for for this notification to get user selections of alternative strings. The `userInfo` dictionary contains the following information:

| Key                      | Value                            |
|--------------------------|----------------------------------|
| `@"NSAlternativeString"` | The selected alternative string. |

