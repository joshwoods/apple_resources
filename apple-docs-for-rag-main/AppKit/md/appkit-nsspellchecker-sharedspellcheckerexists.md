

- AppKit
- NSSpellChecker
-  sharedSpellCheckerExists 

Type Property

# sharedSpellCheckerExists

Returns whether the application’s NSSpellChecker has already been created.

macOS

``` source
class var sharedSpellCheckerExists: Bool { get }
```

## Return Value

true if the shared spell checker already exists, otherwise false.

## See Also

### Getting the Spell Checker

class var shared: NSSpellChecker

Returns the NSSpellChecker (one per application).

