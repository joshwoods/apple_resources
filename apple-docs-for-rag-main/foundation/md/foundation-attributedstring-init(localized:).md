

- Foundation
- AttributedString
-  init(localized:) 

Initializer

# init(localized:)

Creates a localized attributed string from a localized string resource.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(localized resource: LocalizedStringResource)
```

## Parameters 

`resource`  

A LocalizedStringResource that provides the localization key, table, bundle, and locale.

## Discussion

Call this initializer to look up the localization indicated by `resource`. Alter the resource’s locale prior to calling this method if you want to localize this string in a different locale than the process that created the LocalizedStringResource.

The attributed string contains attributes of type AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes to indicate runs containing formatted text, such as localized numbers or dates. Access these attributes with the attribute key localizedNumericArgument or localizedDateArgument.

## See Also

### Creating a Localized Attributed String

init(localized: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?)

Creates an attributed string by looking up a localized string from the app’s bundle.

init&lt;S>(localized: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?, including: S.Type)

Creates an attributed string by looking up a localized string from the app’s bundle, including an attribute scope.

init&lt;S>(localized: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?, including: KeyPath&lt;AttributeScopes, S.Type>)

Creates an attributed string by looking up a localized string from the app’s bundle, including an attribute scope that a key path identifies.

struct LocalizationValue

A reference to a localizable string, with optional string interpolation.

struct FormattingOptions

Options that affect the handling of attributes.

init&lt;S>(localized: LocalizedStringResource, including: S.Type)

Creates a localized attributed string from a localized string resource, including an attribute scope.

init&lt;S>(localized: LocalizedStringResource, including: KeyPath&lt;AttributeScopes, S.Type>)

Creates a localized attributed string from a localized string resource, including an attribute scope that a key path identifies.

struct LocalizedStringResource

A reference to a localizable string, accessible from another process.

