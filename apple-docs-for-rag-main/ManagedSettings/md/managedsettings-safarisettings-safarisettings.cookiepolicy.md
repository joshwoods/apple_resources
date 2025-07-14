

- ManagedSettings
- SafariSettings
-  SafariSettings.CookiePolicy 

Enumeration

# SafariSettings.CookiePolicy

The conditions under which Safari accepts cookies.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum CookiePolicy
```

## Topics

### Accepting Cookies

case always

A policy that indicates the device accepts cookies from all websites.

case currentWebsite

A policy that indicates the device only accepts cookies from the current website.

case never

A policy that indicates the device doesn’t accept cookies from any website.

case visitedWebsites

A policy that indicates the device only accepts cookies from websites in the user’s browsing history.

### Getting the Range

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

var hashValue: Int

func hash(into: inout Hasher)

### Operators

static func &lt; (SafariSettings.CookiePolicy, SafariSettings.CookiePolicy) -> Bool

Returns a Boolean value that indicates whether the value of the first argument is less than that of the second argument.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var description: String

A textual representation of this instance.

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Comparable Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Comparable
- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable

## See Also

### Specifying a Cookie Policy

var cookiePolicy: SafariSettings.CookiePolicy?

Defines the conditions under which Safari accepts cookies.

static let cookiePolicy: SettingMetadata&lt;SafariSettings.CookiePolicy>

The metadata for the setting that configures Safari’s policy for cookies.

