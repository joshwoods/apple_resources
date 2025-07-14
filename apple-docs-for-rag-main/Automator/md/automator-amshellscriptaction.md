

- Automator
-  AMShellScriptAction 

Class

# AMShellScriptAction

An object that represents Automator actions whose runtime behavior is driven by a shell script or by a Perl or Python script.

Mac Catalyst 14.0+macOS 10.4+

``` source
class AMShellScriptAction
```

## Overview

When you create a Shell Script Automator Action project in Xcode, the project template supplies an AMShellScriptAction instance as the Principal Class of the action bundle. This ready-made instance provides a default implementation of the AMAction run(withInput:) method that uses the logic defined in the script. You can substitute your own subclass of AMShellScriptAction for Principal Class if you need to.

## Topics

### Handling the I/O Separator Character

var inputFieldSeparator: String

A string to use as the delimiter between items in the string passed to the action through standard input.

var outputFieldSeparator: String

A string to use as a delimiter in the string output by the action.

var remapLineEndings: Bool

A Boolean value that indicates whether you want automatic remapping of carriage return (`\r`) to newline (`\n`) characters in the input string.

## Relationships

### Inherits From

- AMBundleAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Actions

class AMBundleAction

An object that represents an Automator action that’s a loadable bundle.

class AMAction

An abstract class that defines the interface and general characteristics of Automator actions.

