

- Open Directory
- ODRecord
-  changePassword(\_:toPassword:) 

Instance Method

# changePassword(\_:toPassword:)

Changes the record’s password.

Mac CatalystmacOS 10.6+

``` source
func changePassword(
    _ oldPassword: String!,
    toPassword newPassword: String!
) throws
```

## Parameters 

`oldPassword`  

The record’s old password. Can be `nil` if the user has the proper permissions.

`newPassword`  

The new password.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Authentication

func setNodeCredentials(String!, password: String!) throws

Sets credentials for the record’s node.

func setNodeCredentialsWithRecordType(String!, authenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Sets the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

func verifyExtended(withAuthenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Verifies the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

func verifyPassword(String!) throws

Verifies the password for interaction with the record.

