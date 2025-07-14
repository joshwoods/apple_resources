

- Core Spotlight
- CSLocalizedString
-  init(localizedStrings:) 

Initializer

# init(localizedStrings:)

Initializes a `CSLocalizedString` object with the specified dictionary of localized strings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
init(localizedStrings: [AnyHashable : Any])
```

## Parameters 

`localizedStrings`  

A dictionary in which each key-value pair consists of a language designator and a localized string. For example, you might pass in a dictionary like `@{@"en":@"Email Message"}`.

## Return Value

An object that contains the localized versions for a specific string.

