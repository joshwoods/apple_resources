

- Foundation
- NSScriptSuiteRegistry
-  suite(forAppleEventCode:) 

Instance Method

# suite(forAppleEventCode:)

Returns the name of the suite definition associated with the given four-character Apple event code, `code`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func suite(forAppleEventCode appleEventCode: FourCharCode) -> String?
```

## See Also

### Getting Suite Information

var suiteNames: [String]

Returns the names of the suite definitions currently loaded by the application.

