

- Foundation
- NSScriptSuiteRegistry
-  appleEventCode(forSuite:) 

Instance Method

# appleEventCode(forSuite:)

Returns the Apple event code associated with the suite named `suiteName`, such as `‘core’` for the Core suite.

Mac Catalyst 13.0+macOS 10.0+

``` source
func appleEventCode(forSuite suiteName: String) -> FourCharCode
```

## See Also

### Related Documentation

func suite(forAppleEventCode: FourCharCode) -> String?

Returns the name of the suite definition associated with the given four-character Apple event code, `code`.

### Getting Other Suite Information

func aeteResource(String) -> Data?

Returns an `NSData` object that contains data in `'aete'` resource format describing the scriptability information currently known to the application.

func bundle(forSuite: String) -> Bundle?

Returns the bundle containing the suite-definition property list (extension `.scriptSuite`) identified by `suiteName`.

