

- ManagedApp
- ManagedAppPasswordsProvider
-  identifiers 

Instance Property

# identifiers

An asynchronous sequence of arrays of password identifiers provided by the MDM server.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
var identifiers: some AsyncSequence, Never> { get async }
```

## Discussion

Use password(withIdentifier:) to look up an identifier to obtain the associated password. The sequence yields an array of identifiers when:

- You begin iterating this property using `for await`.

- The list of password identifiers changes.

- The value of one or more passwords changes.

You define the values of the identifiers that an MDM admin can use. Define specific individual values or ranges of values to group passwords, or use the configuration to determine the meaning of the identifiers.

This property yields an empty array if the MDM admin hasn’t provisioned any passwords for your app.

