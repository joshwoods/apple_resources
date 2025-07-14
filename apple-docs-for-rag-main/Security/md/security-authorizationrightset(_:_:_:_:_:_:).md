

- Security
-  AuthorizationRightSet(\_:\_:\_:\_:\_:\_:) 

Function

# AuthorizationRightSet(\_:\_:\_:\_:\_:\_:)

Creates or updates a right entry in the policy database.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationRightSet(
    _ authRef: AuthorizationRef,
    _ rightName: UnsafePointer,
    _ rightDefinition: CFTypeRef,
    _ descriptionKey: CFString?,
    _ bundle: CFBundle?,
    _ localeTableName: CFString?
) -> OSStatus
```

## Parameters 

`authRef`  

A valid authorization reference used to authorize modifications.

`rightName`  

An ASCII character string representing the right name. The policy database does not accept wildcard right names.

`rightDefinition`  

Either a doc://com.apple.documentation/documentation/corefoundation/cfdictionary-rum containing keys defining the rules or a doc://com.apple.documentation/documentation/corefoundation/cfstring-rfh representing the name of another right whose rules you wish to duplicate. See Policy Database Constants for some possible values.

`descriptionKey`  

A string used as a key for looking up localized descriptions. If no localization is found, this is the description itself. This parameter is optional; pass `NULL` if you do not require it.

`bundle`  

A bundle to get localizations from if not the main bundle. This parameter is optional; pass `NULL` if you do not require it.

`localeTableName`  

A string representing a table name from which to get localizations. This parameter is optional; pass `NULL` if you have no localizations or you wish to use the localizations available in `Localizable.strings`.

## Return Value

A result code. See Authorization Services Result Codes.

## Mentioned in 

Extending authorization services with plug-ins

## Discussion

The right you create must be an explicit right with no wildcards. Wildcard rights are for use by system administrators for site configuration. You can use this function to create a new right or modify an existing right. For example:

```
```

adds a rule for letting administrators send faxes. This example creates a right named `“com.ifoo.ifax.send”` and sets the rules to require the user to be an administrator by using the kAuthorizationRuleIsAdmin constant. This example also sets a comment to let the system administrator know that the right authorizes administrators to send a fax.

Because the first parameter is `NULL`, a new AuthorizationRef object is created internally and disposed of. If you need to further use the object (for example, when calling AuthorizationExecuteWithPrivileges), you must explicitly create the object and pass it in as the first argument to AuthorizationRightSet(_:_:_:_:_:_:), then free it with a call to AuthorizationFree(_:_:).

To specify additional attributes for the right, you can pass a dictionary in the `rightDefinition` parameter as shown in the following example.

```
```

This call creates the same right as before, but adds a specific right comment to the rules definition.

When you specify comments, you should be specific about what you need to authorize. For example, the means of proof required for kAuthorizationRuleAuthenticateAsAdmin (a username and password) should not be included here since that rule might be configured differently.

