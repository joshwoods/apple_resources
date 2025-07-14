

- Device Management
- ExtensibleSingleSignOnKerberos
- ExtensibleSingleSignOnKerberos.ExtensionData
-  ExtensibleSingleSignOnKerberos.ExtensionData.DomainRealmMapping 

Device Management Profile

# ExtensibleSingleSignOnKerberos.ExtensionData.DomainRealmMapping

The mapping of realms to their DNS suffixes.

iOS 13.0+iPadOS 13.0+macOS 10.15+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ExtensibleSingleSignOnKerberos.ExtensionData.DomainRealmMapping
```

## Properties

`Realm`

`[string]`

The key should be the name of the realm, and the value is an array of DNS suffixes that map to the realm.

