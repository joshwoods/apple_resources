

- Foundation
- NSScriptSuiteRegistry
-  setShared(\_:) 

Type Method

# setShared(\_:)

Sets the single, shared instance of `NSScriptSuiteRegistry` to `registry`.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func setShared(_ registry: NSScriptSuiteRegistry)
```

## See Also

### Related Documentation

Cocoa Scripting Guide

### Getting and Setting the Shared Instance

class func shared() -> NSScriptSuiteRegistry

Returns the single, shared instance of `NSScriptSuiteRegistry`, creating it first if it doesn’t exist.

