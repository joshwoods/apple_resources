

- System Configuration
-  DHCPClientPreferencesCopyApplicationOptions 

Function

# DHCPClientPreferencesCopyApplicationOptions

Returns the list of options for the specified application ID.

macOS 10.1+

``` source
UInt8 * DHCPClientPreferencesCopyApplicationOptions(CFStringRef applicationID, CFIndex * count);
```

## Parameters 

`applicationID`  

The application’s preference ID (for example, “com.apple.SystemPreferences”).

`count`  

The number of elements in the list of options.

## Return Value

The list of options for the specified application ID, or `NULL` if no options are defined or if an error occurred. Use free(3) to release a non-`NULL` return value.

## See Also

### Group

DHCPClientPreferencesSetApplicationOptions

Updates the DHCP client preferences to include the specified list of options for the specified application ID.

