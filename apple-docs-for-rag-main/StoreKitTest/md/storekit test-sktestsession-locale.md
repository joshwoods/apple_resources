

- StoreKit Test
- SKTestSession
-  locale 

Instance Property

# locale

The value that determines the localization metadata the test environment uses.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var locale: Locale { get set }
```

## Discussion

This value determines the locale the test environment uses when it fetches localized metadata for SKProductsRequest. You provide localized metadata in your StoreKit configuration file.

Changing this property overrides its setting in the StoreKit configuration file for this test session. Call resetToDefaultState() to revert all settings to those in the configuration file.

## See Also

### Configuring the test environment

var storefront: String

The three-letter code that represents the region associated with the App Store storefront.

var disableDialogs: Bool

A Boolean value that determines whether the testing environment disables dialogs during automated testing.

