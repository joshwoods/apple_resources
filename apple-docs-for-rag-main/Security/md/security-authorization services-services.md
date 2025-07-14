

- Security
-  Authorization Services 

API Collection

# Authorization Services

Access restricted areas of the operating system, and control access to particular features of your macOS app.

## Overview

The `Security.Authorization` API is a programming interface to the Security Server and its policy database. This API facilitates access control to restricted areas of the operating system and allows you to restrict a user’s access to particular features in your macOS app. Use authorization services in:

- Software that restricts access to its own tools

- Applications that call system tools

- Software installers that install privileged tools or require access to restricted areas of the operating system

As shown in the image below, the Security Server is a daemon running in the operating system that provides a trusted implementation of various security protocols, including authorization computation. In turn, the Security Server relies on the Security Agent to interface with users when authentication is needed. Thus an app can verify credentials (usernames and passwords) without ever accessing them directly. This authorization process also allows the means of authentication to change in the future (such as adding Touch ID) without your having to modify your app.

Note

For a simplified, class-based version of this API, consider using the SFAuthorization class instead. When you need a user interface that enables display and control of the current authorization state for a particular set of rights, use the SFAuthorizationView class.

Important

The Authorization Services API is not supported within an App Sandbox because the API allows privilege escalation.

## Topics

### Authorization References

func AuthorizationCreate(UnsafePointer&lt;AuthorizationRights>?, UnsafePointer&lt;AuthorizationEnvironment>?, AuthorizationFlags, UnsafeMutablePointer&lt;AuthorizationRef?>?) -> OSStatus

Creates a new authorization reference and provides an option to authorize or preauthorize rights.

func AuthorizationFree(AuthorizationRef, AuthorizationFlags) -> OSStatus

Frees the memory associated with an authorization reference.

struct AuthorizationFlags

The flags used to specify authorization options.

typealias AuthorizationRef

A pointer to an opaque authorization reference structure.

### Authorization Items

Use authorization items (alone or in sets) to represent rights and environment information.

struct AuthorizationItem

A structure containing information about an authorization right or the authorization environment.

struct AuthorizationItemSet

A structure containing a set of authorization items.

typealias AuthorizationRights

An authorization item set designated to represent a set of rights.

typealias AuthorizationEnvironment

An authorization item set designated to hold environment information relevant to authorization decisions.

Authorization Name Tags

Use name tags to define authorization security items.

func AuthorizationFreeItemSet(UnsafeMutablePointer&lt;AuthorizationItemSet>) -> OSStatus

Frees the memory associated with a set of authorization items.

### Rights and Credentials

func AuthorizationCopyInfo(AuthorizationRef, AuthorizationString?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AuthorizationItemSet>?>) -> OSStatus

Retrieves supporting data such as the user name and other information gathered during evaluation of authorization.

func AuthorizationCopyRights(AuthorizationRef, UnsafePointer&lt;AuthorizationRights>, UnsafePointer&lt;AuthorizationEnvironment>?, AuthorizationFlags, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AuthorizationRights>?>?) -> OSStatus

Authorizes and preauthorizes rights synchronously.

func AuthorizationCopyRightsAsync(AuthorizationRef, UnsafePointer&lt;AuthorizationRights>, UnsafePointer&lt;AuthorizationEnvironment>?, AuthorizationFlags, AuthorizationAsyncCallback)

Authorizes and preauthorizes rights asynchronously.

typealias AuthorizationAsyncCallback

A block used as a callback for the asynchronous version of copying authorization rights.

typealias AuthorizationString

A zero-terminated string in UTF-8 encoding.

Authorization Rights Flags

Recognize the values the Security Server sets in an authorization item’s flag field.

### Import and Export

func AuthorizationMakeExternalForm(AuthorizationRef, UnsafeMutablePointer&lt;AuthorizationExternalForm>) -> OSStatus

Creates an external representation of an authorization reference.

func AuthorizationCreateFromExternalForm(UnsafePointer&lt;AuthorizationExternalForm>, UnsafeMutablePointer&lt;AuthorizationRef?>) -> OSStatus

Internalizes the external representation of an authorization reference.

struct AuthorizationExternalForm

The external representation of an authorization reference.

var kAuthorizationExternalFormLength: Int32

The number of bytes in an external form structure’s array.

### The Policy Database

func AuthorizationRightGet(UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CFDictionary?>?) -> OSStatus

Retrieves a right definition as a dictionary.

func AuthorizationRightSet(AuthorizationRef, UnsafePointer&lt;CChar>, CFTypeRef, CFString?, CFBundle?, CFString?) -> OSStatus

Creates or updates a right entry in the policy database.

func AuthorizationRightRemove(AuthorizationRef, UnsafePointer&lt;CChar>) -> OSStatus

Removes a right from the policy database.

Policy Database Constants

Use these constants to set rights and rules in the policy database.

### Result Codes

Authorization Services Result Codes

Recognize result codes specific to the authorization services API.

## See Also

### Related Documentation

Authentication, Authorization, and Permissions Guide

Authorization Services Programming Guide

