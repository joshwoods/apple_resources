

- Security Foundation
- SFAuthorization
-  obtain(withRight:flags:) 

Instance Method

# obtain(withRight:flags:)

Authorizes and preauthorizes one specific right.

macOS 10.10+

``` source
func obtain(
    withRight rightName: AuthorizationString!,
    flags: AuthorizationFlags
) throws
```

## Parameters 

`rightName`  

The name of an authorization right.

`flags`  

A bit mask for specifying authorization options. See obtain(withRights:flags:environment:authorizedRights:) for details about possible flag values.

## Return value

true if operation completes successfully.

## Discussion

Use this method to authorize or preauthorize a single right.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

## See Also

### Authorizing rights

func obtain(withRights: UnsafePointer&lt;AuthorizationRights>!, flags: AuthorizationFlags, environment: UnsafePointer&lt;AuthorizationEnvironment>!, authorizedRights: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AuthorizationRights>?>!) throws

Authorizes and preauthorizes rights to access a privileged operation and returns the granted rights.

