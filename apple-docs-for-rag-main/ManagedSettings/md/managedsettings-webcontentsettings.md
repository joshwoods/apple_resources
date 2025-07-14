

- ManagedSettings
-  WebContentSettings 

Structure

# WebContentSettings

An object that configures which websites a user can access.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct WebContentSettings
```

## Topics

### Filtering Web Domains

var blockedByFilter: WebContentSettings.FilterPolicy?

The current policy for filtering websites.

static let blockedByFilter: SettingMetadata&lt;WebContentSettings.FilterPolicy>

A description of the setting that controls which websites a user can access.

enum FilterPolicy

The policies available for filtering web content based on specific web domains.

## Relationships

### Conforms To

- ManagedSettingsGroup

## See Also

### Restricting Web Content

var safari: SafariSettings

Settings that affect Safari’s search results and cookie policies.

struct SafariSettings

Constraints on Safari’s AutoFill and cookie behaviors.

var webContent: WebContentSettings

Settings that affect web content.

