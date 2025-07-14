

- Authentication Services
- Platform single sign-on (SSO)
- Authentication process
-  Performing a WS-Trust metadata exchange data (MEX) request 

Article

# Performing a WS-Trust metadata exchange data (MEX) request

Send and process a WS-Trust MEX request to determine the version and URLs for authentication.

## Overview

After receiving a preauthentication response from the identity provider (IdP), the next step the system performs for federated authentication with WS-Trust, meaning between security domains, is to send a WS-Trust MEX request to the federated IdP.

The system sends a WS-Trust MEX request to determine the WS-Trust version and URLs to use for authentication. It sends this request when the federationType is ASAuthorizationProviderExtensionLoginConfiguration.FederationType.wsTrust, or when the federationType is ASAuthorizationProviderExtensionLoginConfiguration.FederationType.dynamicWSTrust and the MEX URL is parsed from the preauthentication response. See Performing a preauthentication request for more information.

### Create the WS-Trust MEX network request

The request is an HTTP GET to the URL in federationMEXURL or to the URL received from the pre-authentication request, as shown here:

```
GET /wstrust/mex HTTP/1.1
Host: auth.example.com
```

### Receive the WS-Trust MEX network response

If the http status is `200`, the response body loads as XML. The system parses the XML to determine the WSTrust endpoint and version to use. The system supports WS-Trust versions 2005 and 1.3; however, version 1.3 is preferred. The system only supports https as the transport.

## See Also

### Pre-login

Obtaining a server nonce

Request and process a server nonce to verify communication and detect replays.

Performing a preauthentication request

Request and process a preauthentication for dynamic WS-Trust authentication.

