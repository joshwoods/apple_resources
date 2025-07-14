

- CloudKit
-  Changing Access Controls on User Data 

Article

# Changing Access Controls on User Data

Restrict access to or remove restrictions from a user’s data at their request.

## Overview

Users can ask you to prevent any further changes to their data that your app stores in CloudKit. Use the `restrict` API that CloudKit Web Services provides to honor those requests. You can remove restrictions at the user’s request by calling the `unrestrict` API.

### Identify Containers

To be sure that you restrict changes and access to all of a user’s data that your app stores, cross-reference the list of containers your app has access to in Xcode and assemble a list of those containers’ identifiers. Identifying an App’s Containers describes this process.

The example below stores containers in constants to use later:

```
```

### Create Reusable API Tokens

The `restrict` API call requires a token each time you call the API. You create an API token once for each container in your app using the CloudKit Dashboard, and reuse it in each API call to a specific container.

Generate a token in the CloudKit Dashboard by visiting the page for each container, then selecting API Access \> New Token \> Create Token. Tokens are specific to a deployment environment, so you need separate tokens for the production and development environments.

The example below stores tokens in a dictionary for each container to use later:

```
```

### Create Web Authentication Tokens

The `restrict` API call requires a new authentication token each time you call the API, in addition to the reusable API token. The example below shows how to create that token using an instance of CKFetchWebAuthTokenOperation:

```
```

After you receive the authentication token, you can immediately call the `restrict` API once for each container.

### Restrict Data Access in Each Container

The example below defines the `restrict(container:apiToken:webToken:completionHandler:)` and `requestRestriction(url:completionHandler:)` methods for the example above to build the network request for the `restrict` API:

```
```

### Remove Restrictions

When a user requests that you remove restrictions, you use the `unrestrict` API, which performs the opposite operation that the `restrict` API performs.

The example below shows a modified version of the `restrict(container:apiToken:webToken:completionHandler:)` method from the previous example that removes restrictions instead of enabling them:

```
```

A successful call to the `unrestrict(container:apiToken:webToken: completionHandler:)` function (a `nil` error parameter in the completion handler indicates success) means that your app can access and modify user data.

## See Also

### Privacy

Encrypting User Data

Deploy industry-standard security technologies using CloudKit encryption.

Providing User Access to CloudKit Data

Provide users access to the data your app stores on their behalf.

class CKFetchWebAuthTokenOperation

An operation that creates an authentication token for use with CloudKit web services.

Responding to Requests to Delete Data

Provide options for users to delete their CloudKit data from your app.

Identifying an App’s Containers

Use Xcode’s Project navigator to find the identifiers of active CloudKit containers.

