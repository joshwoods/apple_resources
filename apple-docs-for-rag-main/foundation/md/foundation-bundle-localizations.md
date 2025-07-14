

- Foundation
- Bundle
-  localizations 

Instance Property

# localizations

A list of all the localizations contained in the bundle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var localizations: [String] { get }
```

## Discussion

An array of NSString objects containing language IDs for all the localizations contained in the bundle.

## See Also

### Getting Localization Information

var preferredLocalizations: [String]

An ordered list of preferred localizations contained in the bundle.

var developmentLocalization: String?

The localization for the development language.

var localizedInfoDictionary: [String : Any]?

A dictionary with the keys from the bundle’s localized property list.

class func preferredLocalizations(from: [String]) -> [String]

Returns one or more localizations from the specified list that a bundle object would use to locate resources for the current user.

class func preferredLocalizations(from: [String], forPreferences: [String]?) -> [String]

Returns locale identifiers for which a bundle would provide localized content, given a specified list of candidates for a user’s language preferences.

