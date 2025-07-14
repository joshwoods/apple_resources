

- Roster API
-  Obtaining information about people and classes 

Article

# Obtaining information about people and classes

Prepare your app to request organizational information from a server.

## Overview

Roster API gives you access to information about the people and classes within an Apple School Manager (ASM) organization. To accomplish this, register for access, then perform queries to obtain the users and classes in that organization.

### Plan your integration design

When planning the design for the integration, create roles that allow specific accounts to perform the steps for integrating your app with Roster API. Provide only those roles with the privileges to perform create, read, update, and delete operations for the integration. For example, in ASM, only accounts that have administrator or site-manager roles can authorize an app to use Roster API.

Consider that there’s only one configuration at the organizational level. Accounts belonging to the roles with privileges work with this single configuration. This means that any changes that one privileged account makes are visible to other privileged accounts.

### Select the primary App ID

Use your credentials to log in to the Apple Developer website, then choose Certificates, IDs & Profiles \> Services, and click the Configure button in the Account & Organizational Data Sharing section.

Click the Add button (+) to the right of Configurations, or click the Configure button in the Get Started with Account & Organizational Data Sharing section.

Choose the primary App ID from the drop-down menu, then click Continue.

### Set the return URLs

Return URLs receive the grant code after successfully authorizing with Apple. From the Organizational Data Sharing Scopes options, select Roster API: User access, Roster API: Class access, and Roster API: Test Data access. For more information about the test data access scope, see Validating with the Roster API test scope.

Add your return URLs in the Return URLs section, then enter a URL for the Server to Server Notification Endpoint so you can receive updates about people and accounts.

Review your configuration and click Confirm.

### Generate the client secret

Before you can generate the access token, you’ll first need to generate the client secret, which you’ll need to create the token. See Creating a client secret.

Next, choose an existing key, or create a new key by clicking the Add button (+).

Enter a key name if you’re creating a new key, select Account & Organizational Data Sharing, and click Continue.

Review the information and then click Register to register the key.

Click Download, then set up a client secret. See Creating a client secret.

### Validate using the test scope

To ensure your integration works correctly, test it before providing it to users. See Validating with the Roster API test scope.

### Receive revocation notifications

ASM organizations can set up integration with the supported apps to import information about people and classes.

If an organization decides to revoke an app, Apple sends out a revocation notification to the URL you configures as the Server to Server Notification Endpoint. After receiving the notification, remove all data associated with that organization.

The following is an example revocation notification request:

```
{
    "iss": "https://appleid.apple.com/auth/oauth2/v2"
    "aud": "[CLIENT_ID]",
    "iat": 1508184845,
    "jti": "abede...67890",
    "events": [
        {
            "type": "consent-revoked",
            "sub": "001273.YVlIczRoMFRGbll4ODIzRUV0M2NLNkFRM0VHUTdQ.RVBY",
            "org_id": "8e257987-f221-4171-887d-efead972993b",
            "scopes": "edu.classes.read edu.users.read"
            "event_time": 1508184845
        }
    ]
}
```

Information for `org_id` and `scopes` are part of the payload. Use `org_id` to remove all data associated with the organization.

Use the `/rosterapi/v1/organization` endpoint to determine the `org_id` when obtaining user and class information for an organization. The following is a sample response:

```
{
    "id": "8e257987-f221-4171-887d-efead972993b",
    "type": "EDUCATION",
    "name": "Apple School Manager Test Organization",
    "dateCreated": "2016-07-26T18:11:51Z",
    "dateLastModified": "2016-07-26T18:11:51Z", 
    "domains": [{"name": "mytestschool.org", "isVerified": false}]
}
```

Use `id` as the identifier to associate records to a certain organization. When the revocation notification arrives, delete those records associated with the organization that matches `org_id`.

### Synchronize data with Apple School Manager

Apple synchronizes data in ASM with authorized student information systems every 24 hours. Fetch data using Roster API once every 24 hours to have the most up to date data in your app. If you need to reduce your resource usage, consider fetching data less frequently, for example once every 48 hours or once every week.

Design your synchronization to handle class and roster updates. When someone removes a student from a class in ASM, or deletes a class, subsequent requests to List users in a class and List classes don’t include the removed items. Consider whether to show teachers existing data and give them the option to remove it manually, or automatically remove the deleted records.

## See Also

### Essentials

Validating with the Roster API test scope

Use test data to ensure your integration with the Roster API works correctly.

