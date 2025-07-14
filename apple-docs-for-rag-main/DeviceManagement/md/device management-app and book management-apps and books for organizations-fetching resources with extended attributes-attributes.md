

- Device Management
- App and Book Management
- Apps and Books for Organizations
-  Fetching resources with extended attributes 

Article

# Fetching resources with extended attributes

Specify additional attributes for the API to include in a response.

## Overview

You may want to access some attributes that the server doesn’t fetch unless specifically requested. By default, responses contain only a subset of the available attributes for a resource. The attributes that the server doesn’t fetch by default are known as *extended attributes*. Use the `extend` query parameter to request a set of additional attributes for a resource type.

For example, when fetching an apps resource, you can request that the server add the extended `latestVersionInfo` attribute to the other attributes it returns:

```
GET https://api.ent.apple.com/v1/catalog/{storefront}/stoken-authenticated-apps?ids=1376597908,2001350931&platform=iphone&extend[apps]=latestVersionInfo
```

Available extended attributes include:

- `fileSizeByDevice`

- `languageList`

- `description`

- `latestVersionInfo`

- `privacyPolicyUrl`

- `screenshotsByType`

- `supportURLForLanguage`

- `versionHistory`

- `websiteUrl`

- `requirementsByDeviceFamily`

## See Also

### Essentials

Generating developer tokens

Create a JSON Web Token to authorize your requests to the Apps and Books for Organizations API.

Handling requests and responses

Write a request for app or book metadata and handle responses from the API.

Fetching storefront objects

Pick a region-specific geographic location to retrieve catalog information from.

Common Objects

Understand the common JSON objects that framework responses contain.

