

- Foundation
- NSScriptSuiteRegistry
-  shared() 

Type Method

# shared()

Returns the single, shared instance of `NSScriptSuiteRegistry`, creating it first if it doesn’t exist.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func shared() -> NSScriptSuiteRegistry
```

## Discussion

If it creates an instance, and if the application provides scriptability information in the script suite format, the method loads suite definitions in all frameworks and other bundles that the application currently imports or includes; if information is provided in the sdef format, the method loads information only from the specified sdef file. If in reading scriptability information an exception is `raised` because of parsing errors, it handles the exception by printing a line of information to the console.

## See Also

### Related Documentation

func loadSuite(with: [AnyHashable : Any], from: Bundle)

Loads the suite definition encapsulated in `dictionary`; previously, this suite definition was parsed from a `.scriptSuite` property list contained in a framework or in `bundle`.

### Getting and Setting the Shared Instance

class func setShared(NSScriptSuiteRegistry)

Sets the single, shared instance of `NSScriptSuiteRegistry` to `registry`.

