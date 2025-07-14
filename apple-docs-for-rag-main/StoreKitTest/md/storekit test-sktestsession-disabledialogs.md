

- StoreKit Test
- SKTestSession
-  disableDialogs 

Instance Property

# disableDialogs

A Boolean value that determines whether the testing environment disables dialogs during automated testing.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var disableDialogs: Bool { get set }
```

## Discussion

The default value is `false`. Set this value to `true` when you run automated tests and want to suppress interactive dialogs.

## See Also

### Configuring the test environment

var storefront: String

The three-letter code that represents the region associated with the App Store storefront.

var locale: Locale

The value that determines the localization metadata the test environment uses.

