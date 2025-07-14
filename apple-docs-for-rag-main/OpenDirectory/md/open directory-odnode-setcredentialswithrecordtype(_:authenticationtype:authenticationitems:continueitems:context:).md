

- Open Directory
- ODNode
-  setCredentialsWithRecordType(\_:authenticationType:authenticationItems:continueItems:context:) 

Instance Method

# setCredentialsWithRecordType(\_:authenticationType:authenticationItems:continueItems:context:)

Sets the credentials for interaction with the node using other types of authentication available to Open Directory.

Mac CatalystmacOS 10.6+

``` source
func setCredentialsWithRecordType(
    _ inRecordType: String!,
    authenticationType inType: String!,
    authenticationItems inItems: [Any]!,
    continueItems outItems: AutoreleasingUnsafeMutablePointer!,
    context outContext: AutoreleasingUnsafeMutablePointer!
) throws
```

## Parameters 

`inRecordType`  

The record type that uses the credentials. Can be `nil`. The default value is `kODRecordTypeUsers`.

`inType`  

The authentication type.

`inItems`  

An array of `NSString` or `NSData` objects to be used in the authentication process.

`outItems`  

An array of `NSData` objects returned from the authentication process, if any are returned; `nil` otherwise.

`outContext`  

The proper context if the authentication attempt requires a context; `nil` otherwise. If not `nil`, then more calls must be made with the Context to continue the authentication.

## Discussion

If this function fails, the previous credentials for the node are used.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Setting Node Credentials

func setCredentialsWithRecordType(String!, recordName: String!, password: String!) throws

Sets credentials for interacting with the node.

func setCredentialsUsingKerberosCache(String!) throws

Sets the credentials for interaction with the node using a Kerberos cache.

