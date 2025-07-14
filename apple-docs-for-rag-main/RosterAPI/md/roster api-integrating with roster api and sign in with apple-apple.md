

- Roster API
-  Integrating with Roster API and Sign in with Apple 

Article

# Integrating with Roster API and Sign in with Apple

Associate someone’s Managed Apple ID with their identity in Apple School Manager.

## Overview

When your app uses Sign in with Apple to authenticate someone, Apple checks whether that person’s Managed Apple ID is associated with an Apple School Manager (ASM) organization that’s authorized Roster API for your app. The identity token contains identifiers that you use with Roster API to fetch information about the organization and person.

For more information about decoding an identity token that you receive from Sign in with Apple, see Authenticating users with Sign in with Apple. The decoded identity token is a JSON object with the fields shown in the example below.

```
```

### Compare the organization identifiers

If somebody authenticates with Sign in with Apple using a Managed Apple ID, the decoded identity token includes an `org_id` claim that identifies their organization. Compare the value in token’s `org_id` with the `id` you receive from a Read the organization request. If the two identifiers are equal, then the person who authenticated is a user in an organization that’s authorized Roster API for your app.

### Fetch the user’s record

When the Managed Apple ID is associated with an organization that authorized Roster API for your app, the Sign in with Apple user identifier is the same as their user identifier in Roster API. Get the user identifier from the `sub` value in the decoded identity token, and pass it as the `userId` to a Read a user request.

