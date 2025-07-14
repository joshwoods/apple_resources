

- Security
- Keychain services
- Keychain items
-  Search attribute keys and values 

API Collection

# Search attribute keys and values

Filter a keychain item search.

## Overview

When looking for items using any of the SecItemCopyMatching(_:_:), SecItemUpdate(_:_:), or SecItemDelete(_:) functions, you specify a `query` dictionary containing both the item attributes to look for (see Item attribute keys and values) and additional search attributes that condition the search. For example, you can use the matching key kSecMatchLimit with value kSecMatchLimitOne to restrict the output to include only the first result even when more than one item matches.

## Topics

### Item search matching keys

Keys used to condition a keychain item search.

let kSecMatchPolicy: CFString

A key whose value indicates a policy with which a matching certificate or identity must verify.

let kSecMatchItemList: CFString

A key whose value indicates a list of items to search.

let kSecMatchSearchList: CFString

A key whose value indicates a list of items to search.

let kSecMatchIssuers: CFString

A key whose value is a string to match against a certificate or identity’s issuers.

let kSecMatchEmailAddressIfPresent: CFString

A key whose value is a string to match against a certificate or identity’s email address.

let kSecMatchSubjectContains: CFString

A key whose value is a string to look for in a certificate or identity’s subject.

let kSecMatchSubjectStartsWith: CFString

A key whose value is a string to match against the beginning of a certificate or identity’s subject.

let kSecMatchSubjectEndsWith: CFString

A key whose value is a string to match against the end of a certificate or identity’s subject.

let kSecMatchSubjectWholeString: CFString

A key whose value is a string to exactly match a certificate or identity’s subject.

let kSecMatchCaseInsensitive: CFString

A key whose value is a Boolean indicating whether case-insensitive matching is performed.

let kSecMatchDiacriticInsensitive: CFString

A key whose value is a Boolean indicating whether diacritic-insensitive matching is performed.

let kSecMatchWidthInsensitive: CFString

A key whose value is a Boolean indicating whether width-insensitive matching is performed.

let kSecMatchTrustedOnly: CFString

A key whose value is a Boolean indicating whether untrusted certificates should be returned.

let kSecMatchValidOnDate: CFString

A key whose value indicates the validity date.

let kSecMatchLimit: CFString

A key whose value indicates the match limit.

### Match limit values

Keys used to limit the number of results returned.

let kSecMatchLimitOne: CFString

A value that corresponds to matching exactly one item.

let kSecMatchLimitAll: CFString

A value that corresponds to matching an unlimited number of items.

### Additional item search keys

Keys used to specify additional keychain item search options.

let kSecUseItemList: CFString

A key whose value is an array of items to search.

Deprecated

let kSecUseKeychain: CFString

A key whose value is a keychain to operate on.

let kSecUseOperationPrompt: CFString

A key whose value is an operation prompt.

Deprecated

let kSecUseNoAuthenticationUI: CFString

A key whose value is a Boolean indicating whether to disallow UI authentication.

Deprecated

let kSecUseAuthenticationUI: CFString

A key whose value indicates whether the user is prompted for authentication.

let kSecUseAuthenticationContext: CFString

A key whose value indicates a local authentication context to use.

let kSecUseDataProtectionKeychain: CFString

A key whose value indicates whether to treat macOS keychain items like iOS keychain items.

### UI authentication values

Values you use to indicate whether to allow UI authentication.

let kSecUseAuthenticationUIAllow: CFString

A value that indicates user authentication is allowed.

Deprecated

let kSecUseAuthenticationUIFail: CFString

A value that indicates user authentication is disallowed.

Deprecated

let kSecUseAuthenticationUISkip: CFString

A value that indicates items requiring user authentication should be skipped.

