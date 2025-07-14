

- Foundation
- NSScriptSuiteRegistry
-  classDescriptions(inSuite:) 

Instance Method

# classDescriptions(inSuite:)

Returns the class descriptions contained in the suite identified by `suiteName`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func classDescriptions(inSuite suiteName: String) -> [String : NSScriptClassDescription]?
```

## Discussion

Each class description (instance of NSScriptClassDescription) in the returned dictionary is identified by class name.

## See Also

### Getting and Registering Class Descriptions

func classDescription(withAppleEventCode: FourCharCode) -> NSScriptClassDescription?

Returns the class description associated with the given four-character Apple event code, `code`.

func register(NSScriptClassDescription)

Registers class description `classDescription` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the class name.

