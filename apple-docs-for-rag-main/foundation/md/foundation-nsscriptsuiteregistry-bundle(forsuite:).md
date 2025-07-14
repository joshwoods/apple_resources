

- Foundation
- NSScriptSuiteRegistry
-  bundle(forSuite:) 

Instance Method

# bundle(forSuite:)

Returns the bundle containing the suite-definition property list (extension `.scriptSuite`) identified by `suiteName`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func bundle(forSuite suiteName: String) -> Bundle?
```

## See Also

### Getting Other Suite Information

func aeteResource(String) -> Data?

Returns an `NSData` object that contains data in `'aete'` resource format describing the scriptability information currently known to the application.

func appleEventCode(forSuite: String) -> FourCharCode

Returns the Apple event code associated with the suite named `suiteName`, such as `‘core’` for the Core suite.

