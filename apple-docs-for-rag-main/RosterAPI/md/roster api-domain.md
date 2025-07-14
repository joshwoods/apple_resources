

- Roster API
-  Domain 

Object

# Domain

A DNS domain name associated with an Apple School Manager organization.

Roster API 1.0.0+

``` source
object Domain
```

## Properties

`isVerified`

`boolean`

A flag that indicates whether the domain’s verified in Apple School Manager.

`name`

`string`

The domain name.

## Discussion

An organization can generate Managed Apple IDs in Apple School Manager for the verified domains named in its `Domains` objects. For more information about verifying domains, see Verify domains in Apple Business Manager and Apple School Manager.

## See Also

### Information about the organization

Read the organization

Returns information about the Apple School Manager organization.

object Organization

Information about an Apple School Manager organization.

