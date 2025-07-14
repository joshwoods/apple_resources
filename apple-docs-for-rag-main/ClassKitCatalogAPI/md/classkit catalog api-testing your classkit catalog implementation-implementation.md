

- ClassKit Catalog API
-  Testing Your ClassKit Catalog Implementation 

Article

# Testing Your ClassKit Catalog Implementation

Verify your server interaction before deployment by operating in a development environment.

## Overview

Before you deploy your ClassKit Catalog API changes, you can test them in a development environment that isn’t available to teachers. Use a query parameter in your API calls to choose the development environment, and then use a device in development mode to inspect your updates.

Important

Contexts that you publish in the development environment may be visible to other developers using the development environment in Schoolwork.

### Target the Development Environment

For calls that you make to the ClassKit Catalog API, you set the `environment` query parameter. During normal operation, you set the value of this parameter to `production`. For example, the following `curl` command retrieves the main app context of an example app:

```
% curl -v -X GET "https://classkit-catalog.apple.com/v1/contexts?identifierPath=%5B%22com.apple.example.app%22%5D&locale=en-us&environment=production" -H "Authorization: Bearer "
```

When you want to work with the development environment, set the parameter to `development` instead:

```
% curl -v -X GET "https://classkit-catalog.apple.com/v1/contexts?identifierPath=%5B%22com.apple.example.app%22%5D&locale=en-us&environment=development" -H "Authorization: Bearer "
```

You can read and write the development environment just like the production environment. Data isn’t shared between the two environments.

### Test Your Changes

After uploading content to the development environment, you can inspect the changes. On an iOS device that you use for development, with the Schoolwork app installed, go to Settings \> Developer, and choose ClassKit API.

Then use the ClassKit Catalog Environment section to choose either the Production or Development environment.

When you choose Development, the Schoolwork app on that device shows you data you uploaded to the development environment instead of the production environment data.

## See Also

### Essentials

Authenticating Calls to the ClassKit Catalog API

Establish your identity to the ClassKit Catalog server by providing a cryptographically signed token for each call.

