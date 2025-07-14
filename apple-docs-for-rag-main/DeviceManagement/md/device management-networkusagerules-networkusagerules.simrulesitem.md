

- Device Management
- NetworkUsageRules
-  NetworkUsageRules.SIMRulesItem 

Device Management Profile

# NetworkUsageRules.SIMRulesItem

The policy for individual SIM cards.

iOS 9.0+iPadOS 9.0+Device Assignment ServicesVPP License Management

``` source
object NetworkUsageRules.SIMRulesItem
```

## Properties

`ICCIDs`

`[string]`

 (Required) 

One or more ICCIDs of SIM cards for which the `WiFiAssistPolicy` applies. All ICCIDs in all installed Network Usage Rules payloads must be unique. An example ICCID is `89310410106543789301`.

`WiFiAssistPolicy`

`integer`

 (Required) 

The Wi-Fi Assist policy to apply to the SIM cards specified in the ICCIDs. Allowed values:

`2`  
Use the default system policy for the specified SIM card(s).

Possible Values: `2, 3`

## Overview

`3`  
Make Wi-Fi Assist switch more aggressively from a poor Wi-Fi connection to cellular data for the specified SIM card(s). This setting may increase cellular data use and may impact battery life.

For more information, see About Wi-Fi Assist.

## See Also

### Objects

object NetworkUsageRules.ApplicationRulesItem

The application rules dictionary.

