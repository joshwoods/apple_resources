

- CKTool JS
-  Security 

Structure

# Security

A dictionary of your authorization tokens.

CKTool JS 1.2.15+

``` source
dictionary Security {
 string? CloudKitAPITokenAuth;
 string? CloudKitWebAuthTokenAuth;
 string? ManagementTokenAuth;
 string? UserTokenAuth;
};
```

## Overview

A dictionary that contains your management token, user token, or CloudKit tokens.

You pass this dictionary when creating an instance of a promises API class as one of its property values.

## Topics

### Instance Properties

CloudKitAPITokenAuth

Your CloudKit API token.

CloudKitWebAuthTokenAuth

Your CloudKit Web Authentication token.

ManagementTokenAuth

Your management token.

UserTokenAuth

Your user token.

## See Also

### Initialization

PromisesApi

Creates a `PromisesApi` object.

PromisesApiOptions

A dictionary of options for promises API classes.

