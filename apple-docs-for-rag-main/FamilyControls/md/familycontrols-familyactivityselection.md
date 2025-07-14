

- FamilyControls
-  FamilyActivitySelection 

Structure

# FamilyActivitySelection

A collection of applications, categories, and web domains selected by the user.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct FamilyActivitySelection
```

## Overview

To protect the user’s privacy, `FamilyActivitySelection` holds opaque values that represent categories, applications, and web domains selected by the user.

You can then pass these opaque values to instances and methods from the ManagedSettings and DeviceActivity frameworks to set up and manage parental controls.

Important

If a user, parent, or guardian revokes authorization of your app, any tokens that FamilyActivitySelection provided while your app was authorized are voided.

For more information on prompting the user to select items, see FamilyActivityPicker.

## Topics

### Accessing Selected Categories

var categories: Set&lt;ActivityCategory>

A set of category instances selected by the user.

var categoryTokens: Set&lt;ActivityCategoryToken>

Tokens that represent categories selected by the user.

### Accessing Selected Applications

var applications: Set&lt;Application>

A set of application instances selected by the user.

var applicationTokens: Set&lt;ApplicationToken>

Tokens that represent applications selected by the user.

### Accessing Selected Web Domains

var webDomains: Set&lt;WebDomain>

A set of web domain instances selected by the user.

var webDomainTokens: Set&lt;WebDomainToken>

Tokens that represent web domains selected by the user.

### Creating Activity Selections

init()

Creates a new activity selection instance.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Encoding Activity Selections

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Comparing Activity Selections

static func == (FamilyActivitySelection, FamilyActivitySelection) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two activity selections aren’t equal.

### Initializers

init(includeEntireCategory: Bool)

Creates a new activity selection instance.

### Instance Properties

let includeEntireCategory: Bool

A Boolean value that indicates whether the selection should include applications and web domains from the selected categories.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable

## See Also

### User-Selected Apps and Web Domains

struct FamilyActivityPicker

A view in which users specify applications, web domains, and categories without revealing their choices to the app.

