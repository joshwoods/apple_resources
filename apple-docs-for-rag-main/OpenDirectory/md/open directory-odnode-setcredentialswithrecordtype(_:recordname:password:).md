

- Open Directory
- ODNode
-  setCredentialsWithRecordType(\_:recordName:password:) 

Instance Method

# setCredentialsWithRecordType(\_:recordName:password:)

Sets credentials for interacting with the node.

Mac CatalystmacOS 10.6+

``` source
func setCredentialsWithRecordType(
    _ inRecordType: String!,
    recordName inRecordName: String!,
    password inPassword: String!
) throws
```

## Parameters 

`inRecordType`  

The record type that uses the credentials. Can be `nil`. The default value is `kODRecordTypeUsers`.

`inRecordName`  

The username to use to authenticate with the node.

`inPassword`  

The password to use to authenticate with the node.

## Discussion

If this function fails, the previous credentials for the node are used.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Setting Node Credentials

func setCredentialsWithRecordType(String!, authenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Sets the credentials for interaction with the node using other types of authentication available to Open Directory.

func setCredentialsUsingKerberosCache(String!) throws

Sets the credentials for interaction with the node using a Kerberos cache.

