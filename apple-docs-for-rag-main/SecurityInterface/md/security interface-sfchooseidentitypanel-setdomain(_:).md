

- Security Interface
- SFChooseIdentityPanel
-  setDomain(\_:) 

Instance Method

# setDomain(\_:)

Sets an optional domain in which the identity is to be used.

macOS 10.5+

``` source
@MainActor
func setDomain(_ domainString: String!)
```

## Parameters 

`domainString`  

A string containing a hostname, RFC 822 name (email address), URL, or similar identifier.

## Discussion

Call this method to associate a domain with the chosen identity. If the user chooses an identity and a domain is set, an identity preference item is created in the default keychain. Subsequent calls to SecIdentitySearchCreate and SecIdentitySearchCopyNext return the preferred identity for this domain first.

## See Also

### Working with Domains

func domain() -> String!

Returns the domain that will be associated with the chosen identity.

