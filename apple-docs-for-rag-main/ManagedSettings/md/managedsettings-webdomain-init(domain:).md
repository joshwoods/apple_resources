

- ManagedSettings
- WebDomain
-  init(domain:) 

Initializer

# init(domain:)

Creates an object that represents the specified web domain.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(domain: String)
```

## Parameters 

`domain`  

A website to allow or block.

## Discussion

Provide a high-level domain, such as `example.com`. To protect a family’s privacy, use init(token:) instead.

## See Also

### Creating a Web Domain

init(token: WebDomainToken)

Creates an object that represents the provided domain.

