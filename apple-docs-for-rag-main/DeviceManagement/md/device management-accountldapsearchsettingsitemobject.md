

- Device Management
-  AccountLDAPSearchSettingsItemObject 

Object

# AccountLDAPSearchSettingsItemObject

The settings for configuring the search behavior with an LDAP server.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object AccountLDAPSearchSettingsItemObject
```

## Properties

`Scope`

`string`

The type of recursion to use in the search.

- `Base`: Only the `SearchBase` node.

- `OneLevel`: The `SearchBase` node and its immediate children.

- `Subtree`: The `SearchBase` node and all its chidren, regardless of depth.

Default: `Subtree`

Possible Values: `Base, OneLevel, Subtree`

`SearchBase`

`string`

 (Required) 

The path to the node where a search starts. For example, `ou=people,o=example corp`.

`VisibleDescription`

`string`

The description of this search setting in the Contacts and Settings apps. If not present, the apps display no name.

