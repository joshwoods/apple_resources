

- Foundation
- NSScriptSuiteRegistry
-  commandDescription(withAppleEventClass:andAppleEventCode:) 

Instance Method

# commandDescription(withAppleEventClass:andAppleEventCode:)

Returns the command description identified by a suite’s four-character Apple event code of the class (`eventClass`) and the four-character Apple event code of the command (`commandCode`).

Mac Catalyst 13.0+macOS 10.0+

``` source
func commandDescription(
    withAppleEventClass appleEventClassCode: FourCharCode,
    andAppleEventCode appleEventIDCode: FourCharCode
) -> NSScriptCommandDescription?
```

## See Also

### Getting and Registering Command Descriptions

func commandDescriptions(inSuite: String) -> [String : NSScriptCommandDescription]?

Returns the command descriptions contained in the suite identified by `suiteName`.

func register(NSScriptCommandDescription)

Registers command description `commandDesc` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the command name.

