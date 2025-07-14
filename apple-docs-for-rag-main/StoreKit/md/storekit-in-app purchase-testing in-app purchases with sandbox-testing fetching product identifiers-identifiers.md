

- StoreKit
- In-App Purchase
- Testing In-App Purchases with sandbox
-  Testing fetching product identifiers 

Article

# Testing fetching product identifiers

Verify that your app receives the correct product identifiers by inspecting or replicating your app’s process for retrieving the identifiers.

## Overview

If you embed your product identifiers in your app, set a breakpoint in your code after the code loads the identifiers. Verify that the instance of NSArray contains your expected list of product identifiers.

Note

Changes that you make to product metadata in App Store Connect can take up to one hour to appear in the sandbox environment.

If your app fetches your product identifiers from a server, manually fetch the JSON file using a web browser such as Safari, or a command-line utility such as `curl`. Verify that the data your server returns contains the expected list of product identifiers and that your server correctly implements standard HTTP caching mechanisms.

For more information on fetching product identifiers, see Loading in-app product identifiers.

## See Also

### Product identifiers and requests

Testing invalid product identifier handling

Verify that your app correctly handles invalid product identifiers.

Testing a product request

Verify that requests for products function properly in the sandbox environment by inspecting the App Store response.

