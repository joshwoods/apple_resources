

- CKTool JS
- AuthenticationRequiredError
-  redirectUrl 

Instance Property

# redirectUrl

A redirect URL for the user to securely sign in using their Apple ID.

CKTool JS 1.2.15+

``` source
attribute string redirectUrl;
```

## Discussion

The Apple authentication service presents the actual sign-in page through this redirect URL so that the user’s credentials remain confidential.

