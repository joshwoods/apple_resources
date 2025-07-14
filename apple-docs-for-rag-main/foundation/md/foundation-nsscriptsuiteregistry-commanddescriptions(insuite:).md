

- Foundation
- NSScriptSuiteRegistry
-  commandDescriptions(inSuite:) 

Instance Method

# commandDescriptions(inSuite:)

Returns the command descriptions contained in the suite identified by `suiteName`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func commandDescriptions(inSuite suiteName: String) -> [String : NSScriptCommandDescription]?
```

## Discussion

Each command description (instance of NSScriptCommandDescription) in the returned dictionary is identified by command name.

## See Also

### Getting and Registering Command Descriptions

func commandDescription(withAppleEventClass: FourCharCode, andAppleEventCode: FourCharCode) -> NSScriptCommandDescription?

Returns the command description identified by a suite’s four-character Apple event code of the class (`eventClass`) and the four-character Apple event code of the command (`commandCode`).

func register(NSScriptCommandDescription)

Registers command description `commandDesc` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the command name.

