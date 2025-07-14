

- Core Spotlight
-  CSLocalizedString 

Class

# CSLocalizedString

An object that displays localized text in search results related to your app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class CSLocalizedString
```

## Overview

The `CSLocalizedString` class helps you localize text in searchable items. You can use a `CSLocalizedString` object in place of an NSString object to display localized text in search results related to your app.

For example, you might use the following code to define a `CSLocalizedString` object for a searchable item you want to identify as “Song” in English:

```
CSSearchableItem *item = [CSSearchableItem new];
    item.uniqueIdentifier = @"song";

    CSSearchableItemAttributeSet *attributes = [[CSSearchableItemAttributeSet alloc] initWithItemContentType:(NSString *)kUTTypeItem];
    item.attributeSet = attributes;

    CSLocalizedString *displayName = [[CSLocalizedString alloc] initWithLocalizedStrings:@{@"en":@"Song", @"fr":@"Chanson"}];
    attributes.displayName = displayName.localizedString;
```

## Topics

### Specifying localized strings

init(localizedStrings: [AnyHashable : Any])

Initializes a `CSLocalizedString` object with the specified dictionary of localized strings.

### Getting a localized string

func localizedString() -> String

Returns the localized string for the current language.

## Relationships

### Inherits From

- NSString

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Searchable items

class CSSearchableItem

The details of your app-specific content that someone might search for on their devices.

class CSSearchableItemAttributeSet

The detailed metadata for a searchable item.

class CSCustomAttributeKey

A key associated with a custom attribute for a searchable item.

class CSPerson

An object that represents a person in the context of search results.

