

- StoreKit Test
- SKTestSession
-  storefront 

Instance Property

# storefront

The three-letter code that represents the region associated with the App Store storefront.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var storefront: String { get set }
```

## Discussion

This property uses the ISO 3166-1 alpha-3 region code representation. The default value is `USA`.

In the testing environment, this variable determines the value of the storefront variable on your app’s payment queue, and affects the currency type displayed in the payment sheet.

Changing this property overrides its setting in the StoreKit configuration file for this test session. Call resetToDefaultState() to revert all settings to those in the configuration file.

## See Also

### Configuring the test environment

var locale: Locale

The value that determines the localization metadata the test environment uses.

var disableDialogs: Bool

A Boolean value that determines whether the testing environment disables dialogs during automated testing.

