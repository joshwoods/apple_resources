

- Device Management
- LDAP
-  LDAP.LDAPSearchSettingsItem 

Device Management Profile

# LDAP.LDAPSearchSettingsItem

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object LDAP.LDAPSearchSettingsItem
```

## Properties

`LDAPSearchSettingDescription`

`string`

The description of this search setting.

`LDAPSearchSettingScope`

`string`

The type of recursion to use in the search. Allowed values:

`LDAPSearchSettingScopeBase`  
Only the immediate node that the search base points to

Default: `LDAPSearchSettingScopeSubtree`

Possible Values: `LDAPSearchSettingScopeBase, LDAPSearchSettingScopeOneLevel, LDAPSearchSettingScopeSubtree`

`LDAPSearchSettingSearchBase`

`string`

 (Required) 

## Overview

`LDAPSearchSettingScopeOneLevel`  
The node plus its immediate children

`LDAPSearchSettingScopeSubtree`  
The node plus all children, regardless of depth

- LDAPSearchSettingSearchBase: The path to the node where a search should start.

