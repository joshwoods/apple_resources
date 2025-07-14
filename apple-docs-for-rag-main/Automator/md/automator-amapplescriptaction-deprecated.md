

- Automator
-  AMAppleScriptAction Deprecated

Class

# AMAppleScriptAction

An object that represents Automator actions whose runtime behavior is driven by an AppleScript script.

Mac Catalyst 14.0+macOS 10.4+

``` source
class AMAppleScriptAction
```

Deprecated

Use the Cocoa-AppleScript template (an instance of AMBundleAction) in Xcode to create AppleScript-based Automator actions.

## Overview

An AMAppleScriptAction object holds the compiled script as an instance of the `OSAScript` class. By default, the `OSAScript` object is instantiated from the script in the Xcode project file `main.applescript`.

When you create a Automator Applescript Action project in Xcode, the project template supplies an AMAppleScriptAction instance as File’s Owner of the action bundle. This ready-made instance provides a default implementation of the AMAction run(withInput:) method that uses the logic defined in the script. You can substitute your own subclass of AMAppleScriptAction for File’s Owner if you need to.

## Topics

### Accessing the script

var script: OSAScript?

An `OSAScript` object representing the receiver’s script containing the `on run` command handler.

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

