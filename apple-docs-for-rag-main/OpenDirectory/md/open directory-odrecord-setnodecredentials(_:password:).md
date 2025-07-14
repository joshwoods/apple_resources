

- Open Directory
- ODRecord
-  setNodeCredentials(\_:password:) 

Instance Method

# setNodeCredentials(\_:password:)

Sets credentials for the record’s node.

Mac CatalystmacOS 10.6+

``` source
func setNodeCredentials(
    _ inUsername: String!,
    password inPassword: String!
) throws
```

## Parameters 

`inUsername`  

The username to use to authenticate with the node.

`inPassword`  

The password to use to authenticate with the node.

## Discussion

If this function fails, the previous credentials for the node are used.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Authentication

func changePassword(String!, toPassword: String!) throws

Changes the record’s password.

func setNodeCredentialsWithRecordType(String!, authenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Sets the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

func verifyExtended(withAuthenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Verifies the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

func verifyPassword(String!) throws

Verifies the password for interaction with the record.

