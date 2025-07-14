

- Foundation
- URL Loading System
-  Handling an authentication challenge 

# Handling an authentication challenge

Respond appropriately when a server demands authentication for a URL request.

## Overview

When your app makes a request with a URLSessionTask, the server may respond with one or more demands for credentials before continuing. The session task attempts to handle this for you. If it can’t, it calls your session’s delegate to handle the challenges.

Implement the delegate methods described in this article to answer challenges issued by a server that your app connects to. If you don’t implement a delegate, your request may be denied by the server, and you receive a response with HTTP status code `401` (Forbidden) instead of the data you expect.

### Determine the appropriate delegate method

Implement one or both delegate authentication methods, depending on the nature of the challenge(s) you receive.

- Implement the urlSession(_:didReceive:completionHandler:) method of URLSessionDelegate to handle session-wide challenges. These are challenges like Transport Layer Security (TLS) validation. Once you’ve successfully handled this kind of challenge, your action remains in effect for all tasks created from that URLSession.

- Implement the urlSession(_:task:didReceive:completionHandler:) method of URLSessionTaskDelegate to handle task-specific challenges. These are challenges like demands for username/password authentication. Each task created from a given session may issue its own challenges.

Note

See NSURLProtectionSpace authentication method constants for a guide to which authentication methods are session-wide or task-specific.

As a simple example, consider what happens when you request an `http` URL protected by HTTP Basic authentication, as defined in RFC 7617. Because this is a task-specific challenge, you handle this by implementing urlSession(_:task:didReceive:completionHandler:).

Note

If you connect via `https`, you also receive a server trust challenge. See Performing manual server trust authentication for information on handling this type of session-wide challenge.

Figure 1 outlines a strategy for responding to the HTTP Basic challenge.

The following sections implement this strategy.

### Determine the type of authentication challenge

When you receive an authentication challenge, use your delegate method to determine the type of challenge. The delegate method receives a URLAuthenticationChallenge instance that describes the challenge being issued. This instance contains a protectionSpace property whose authenticationMethod property indicates the kind of challenge being issued (such as a request for a username and password, or a client certificate). You use this value to determine whether you can handle the challenge.

You respond to the challenge by directly invoking the completion handler passed in to the challenge, passing an URLSession.AuthChallengeDisposition indicating your response to the challenge. You use the disposition argument to provide a credential, cancel the request, or allow the default handling to proceed, whichever is appropriate.

doc:handling-an-authentication-challenge#Listing-1 tests the authentication method to see if it is the expected type, HTTP Basic. If the `authenticationMethod` property indicates some other kind of challenge, it calls the completion handler with the URLSession.AuthChallengeDisposition.performDefaultHandling disposition. Telling the task to use its default handling may satisfy the challenge; otherwise, the task will move on to the next challenge in the response and call this delegate again. This process continues until the task reaches the HTTP Basic challenge that you expect to handle.

Listing 1. Checking the authentication method of an authentication challenge

```
let authMethod = challenge.protectionSpace.authenticationMethod
guard authMethod == NSURLAuthenticationMethodHTTPBasic else {
    completionHandler(.performDefaultHandling, nil)
    return
}
```

### Create a credential instance

To successfully answer the challenge, you need to submit a credential appropriate to type of challenge you have received. For HTTP Basic and HTTP Digest challenges, you provide a username and password. doc:handling-an-authentication-challenge#Listing-2 shows a helper method that attempts to create a URLCredential instance from user-interface fields, if they are filled in.

Listing 2. Creating a URLCredential from user interface values

```
func credentialsFromUI() -> URLCredential? {
    guard let username = usernameField.text, !username.isEmpty,
        let password = passwordField.text, !password.isEmpty else {
            return nil
    }
    return URLCredential(user: username, password: password,
                         persistence: .forSession)
}
```

In this example, the returned URLCredential has URLCredential.Persistence.forSession persistence, so it’s only stored by the URLSession instance that created the task. You would need to supply new URLCredential instances for tasks created by other session instances, and on future runs of the app.

### Call the completion handler

Once you’ve tried to create a credential instance, you must call the completion handler to answer the challenge.

- If you can’t create a credential, or if the user explicitly canceled, call the completion handler and pass the URLSession.AuthChallengeDisposition.cancelAuthenticationChallenge disposition.

- If you can create a credential instance, use the URLSession.AuthChallengeDisposition.useCredential disposition to pass it to the completion handler.

doc:handling-an-authentication-challenge#Listing-3 shows both these options.

Listing 3. Invoking the authentication challenge completion Handler

```
guard let credential = credentialOrNil else {
    completionHandler(.cancelAuthenticationChallenge, nil)
    return
}
completionHandler(.useCredential, credential)
```

If you supply a credential that is accepted by the server, the task begins uploading or downloading data.

Important

You can pass the completion handler to other methods or temporarily store it in a property, for situations like waiting for the user to complete a username/password dialog. But eventually you must call the completion handler to complete the challenge and allow the task to proceed, even if you’re choosing to cancel, as seen in the failure case of doc:handling-an-authentication-challenge#Listing-3.

### Handle failures gracefully

If the credential is refused, the system calls your delegate method again. When this happens, the callback provides your rejected credential as the proposedCredential property of the URLAuthenticationChallenge parameter. The challenge instance also includes a previousFailureCount property, which indicates how many times the credential has been rejected. You can use these properties to determine what to do next. For example, if the previousFailureCount is greater than zero, you could use the user string of the proposedCredential to populate a user/password reentry UI.

## Topics

### Creating URL credentials

Performing manual server trust authentication

Evaluate the server’s security credentials in your app.

## See Also

### Authentication and credentials

class URLAuthenticationChallenge

A challenge from a server requiring authentication from the client.

class URLCredential

`A`n authentication credential consisting of information specific to the type of credential and the type of persistent storage to use, if any.

class URLCredentialStorage

The manager of a shared credentials cache.

class URLProtectionSpace

A server or an area on a server, commonly referred to as a realm, that requires authentication.

