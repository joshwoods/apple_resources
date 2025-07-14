

- Foundation
- NSScriptSuiteRegistry
-  register(\_:) 

Instance Method

# register(\_:)

Registers class description `classDescription` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the class name.

Mac Catalyst 13.0+macOS 10.0+

``` source
func register(_ classDescription: NSScriptClassDescription)
```

## See Also

### Related Documentation

func loadSuite(with: [AnyHashable : Any], from: Bundle)

Loads the suite definition encapsulated in `dictionary`; previously, this suite definition was parsed from a `.scriptSuite` property list contained in a framework or in `bundle`.

func register(NSScriptCommandDescription)

Registers command description `commandDesc` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the command name.

### Getting and Registering Class Descriptions

func classDescriptions(inSuite: String) -> [String : NSScriptClassDescription]?

Returns the class descriptions contained in the suite identified by `suiteName`.

func classDescription(withAppleEventCode: FourCharCode) -> NSScriptClassDescription?

Returns the class description associated with the given four-character Apple event code, `code`.

