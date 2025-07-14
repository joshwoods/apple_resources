

- Open Directory
- ODRecord
-  verifyExtended(withAuthenticationType:authenticationItems:continueItems:context:) 

Instance Method

# verifyExtended(withAuthenticationType:authenticationItems:continueItems:context:)

Verifies the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

Mac CatalystmacOS 10.6+

``` source
func verifyExtended(
    withAuthenticationType inType: String!,
    authenticationItems inItems: [Any]!,
    continueItems outItems: AutoreleasingUnsafeMutablePointer!,
    context outContext: AutoreleasingUnsafeMutablePointer!
) throws
```

## Parameters 

`inType`  

The authentication type.

`inItems`  

An array of `NSString` or `NSData` objects to be used in the authentication process.

`outItems`  

An array of `NSData` objects returned from the authentication process, if any are returned; `nil` otherwise.

`outContext`  

The proper context if the authentication attempt requires a context; `nil` otherwise. If not `nil`, then more calls must be made with the Context to continue the authentication.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Authentication

func changePassword(String!, toPassword: String!) throws

Changes the record’s password.

func setNodeCredentials(String!, password: String!) throws

Sets credentials for the record’s node.

func setNodeCredentialsWithRecordType(String!, authenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Sets the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

func verifyPassword(String!) throws

Verifies the password for interaction with the record.

