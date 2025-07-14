

- Foundation
- NSScriptSuiteRegistry
-  loadSuite(with:from:) 

Instance Method

# loadSuite(with:from:)

Loads the suite definition encapsulated in `dictionary`; previously, this suite definition was parsed from a `.scriptSuite` property list contained in a framework or in `bundle`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func loadSuite(
    with suiteDeclaration: [AnyHashable : Any],
    from bundle: Bundle
)
```

## Discussion

The method extracts information from the dictionary and caches it in various internal collection objects. If keys are missing or values are of the wrong type, it logs messages to the console. It also registers class descriptions and command descriptions. In registering a class description, it invokes the NSClassDescription class method register(_:for:). In registering a command description, it arranges for the Apple event translator to handle incoming Apple events that represent the defined commands.

This method is invoked when the shared instance is initialized and when bundles are loaded at runtime. Prior to invoking it, `NSScriptSuiteRegistry` creates the dictionary argument from the `.scriptSuite` property list. If you invoke this method in your code, you should try to do it before the application receives its first Apple event.

## See Also

### Related Documentation

func register(NSScriptClassDescription)

Registers class description `classDescription` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the class name.

class func shared() -> NSScriptSuiteRegistry

Returns the single, shared instance of `NSScriptSuiteRegistry`, creating it first if it doesn’t exist.

func register(NSScriptCommandDescription)

Registers command description `commandDesc` for use by Cocoa’s built-in scripting support by storing it in a per-suite internal dictionary under the command name.

### Loading Suites

func loadSuites(from: Bundle)

Loads the suite definitions in bundle `aBundle`, invoking loadSuite(with:from:) for each suite found.

