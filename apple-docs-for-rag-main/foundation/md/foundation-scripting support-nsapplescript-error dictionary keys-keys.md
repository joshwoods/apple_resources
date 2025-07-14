

- Foundation
- Scripting Support
- NSAppleScript
-  Error Dictionary Keys 

API Collection

# Error Dictionary Keys

If the result of init(contentsOf:error:), compileAndReturnError(_:), executeAndReturnError(_:), or executeAppleEvent(_:error:), signals failure (`nil`, false, `nil`, or `nil`, respectively), a pointer to an autoreleased dictionary is put at the location pointed to by the error parameter. The error info dictionary may contain entries that use any combination of the following keys, including no entries at all.

## Topics

### Constants

class let errorMessage: String

An `NSString` that supplies a detailed description of the error condition.

class let errorNumber: String

An `NSNumber` that specifies the error number.

class let errorAppName: String

An `NSString` that specifies the name of the application that generated the error.

class let errorBriefMessage: String

An `NSString` that provides a brief description of the error.

class let errorRange: String

An `NSValue` that specifies a range.

