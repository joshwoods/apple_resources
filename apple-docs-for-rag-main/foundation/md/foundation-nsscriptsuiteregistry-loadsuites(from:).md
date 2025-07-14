

- Foundation
- NSScriptSuiteRegistry
-  loadSuites(from:) 

Instance Method

# loadSuites(from:)

Loads the suite definitions in bundle `aBundle`, invoking loadSuite(with:from:) for each suite found.

Mac Catalyst 13.0+macOS 10.0+

``` source
func loadSuites(from bundle: Bundle)
```

## Discussion

If errors occur while method is parsing a suite-definition file, the method logs error messages to the console.

## See Also

### Loading Suites

func loadSuite(with: [AnyHashable : Any], from: Bundle)

Loads the suite definition encapsulated in `dictionary`; previously, this suite definition was parsed from a `.scriptSuite` property list contained in a framework or in `bundle`.

