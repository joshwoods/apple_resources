

- Core Foundation
- CFError
-  Keys for the user info dictionary 

API Collection

# Keys for the user info dictionary

Keys in the `userInfo` dictionary.

## Overview

When you create a user info dictionary, at a minimum you should provide values for one of `kCFErrorLocalizedDescriptionKey` and `kCFErrorLocalizedFailureReasonKey`; ideally you should provide values for `kCFErrorLocalizedDescriptionKey`, `kCFErrorLocalizedFailureReasonKey`, and `kCFErrorLocalizedRecoverySuggestionKey`. Typically, you should provide a value for one of either `kCFErrorURLKey` or `kCFErrorFilePathKey`.

## Topics

### Constants

let kCFErrorLocalizedDescriptionKey: CFString!

Key to identify the user-presentable description in the `userInfo` dictionary.

let kCFErrorLocalizedFailureReasonKey: CFString!

Key to identify the user-presentable failure reason in the `userInfo` dictionary.

let kCFErrorLocalizedRecoverySuggestionKey: CFString!

Key to identify the user-presentable recovery suggestion in the `userInfo` dictionary.

let kCFErrorDescriptionKey: CFString!

Key to identify the description in the `userInfo` dictionary.

let kCFErrorUnderlyingErrorKey: CFString!

Key to identify the underlying error in the `userInfo` dictionary.

let kCFErrorURLKey: CFString!

Key to identify associated URL in the `userInfo` dictionary.

let kCFErrorFilePathKey: CFString!

Key to identify associated file path in the `userInfo` dictionary.

## See Also

### Constants

Error domains

These constants define domains for CFError objects.

