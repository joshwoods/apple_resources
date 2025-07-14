

- Open Directory
- ODRecord
-  verifyPassword(\_:) 

Instance Method

# verifyPassword(\_:)

Verifies the password for interaction with the record.

Mac CatalystmacOS 10.6+

``` source
func verifyPassword(_ inPassword: String!) throws
```

## Parameters 

`inPassword`  

The password for authenticating with the record.

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

func verifyExtended(withAuthenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Verifies the credentials for interaction with the record’s node using other types of authentication available to Open Directory.

