

- Foundation
- NSScriptSuiteRegistry
-  register(\_:) 

Instance Method

# register(\_:)

Registers command description `commandDesc` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the command name.

Mac Catalyst 13.0+macOS 10.0+

``` source
func register(_ commandDescription: NSScriptCommandDescription)
```

## Discussion

Also registers with the single, shared instance of NSAppleEventManager to handle incoming Apple events that should be handled by the command.

## See Also

### Related Documentation

func register(NSScriptClassDescription)

Registers class description `classDescription` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the class name.

func loadSuite(with: [AnyHashable : Any], from: Bundle)

Loads the suite definition encapsulated in `dictionary`; previously, this suite definition was parsed from a `.scriptSuite` property list contained in a framework or in `bundle`.

### Getting and Registering Command Descriptions

func commandDescriptions(inSuite: String) -> [String : NSScriptCommandDescription]?

Returns the command descriptions contained in the suite identified by `suiteName`.

func commandDescription(withAppleEventClass: FourCharCode, andAppleEventCode: FourCharCode) -> NSScriptCommandDescription?

Returns the command description identified by a suite’s four-character Apple event code of the class (`eventClass`) and the four-character Apple event code of the command (`commandCode`).

