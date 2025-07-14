

- Open Directory
- ODNode
-  setCredentialsUsingKerberosCache(\_:) 

Instance Method

# setCredentialsUsingKerberosCache(\_:)

Sets the credentials for interaction with the node using a Kerberos cache.

Mac CatalystmacOS 10.6+

``` source
func setCredentialsUsingKerberosCache(_ inCacheName: String!) throws
```

## Parameters 

`inCacheName`  

The name of the Kerberos cache.

## Discussion

If this function fails, the previous credentials for the node are used.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Setting Node Credentials

func setCredentialsWithRecordType(String!, recordName: String!, password: String!) throws

Sets credentials for interacting with the node.

func setCredentialsWithRecordType(String!, authenticationType: String!, authenticationItems: [Any]!, continueItems: AutoreleasingUnsafeMutablePointer&lt;NSArray?>!, context: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>!) throws

Sets the credentials for interaction with the node using other types of authentication available to Open Directory.

