

- Social
- SLComposeViewController
-  init(forServiceType:) 

Initializer

# init(forServiceType:)

Creates a new social compose view controller.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
init!(forServiceType serviceType: String!)
```

## Parameters 

`serviceType`  

This specifies the social networking service to which you want to post. You must use one of the possible values listed in Service Type Constants. This also sets the value of serviceType. If an invalid `serviceType` is passed in, this method throws an exception.

## Return Value

Returns a social compose view controller or `nil` if an error occurs.

## Discussion

Use this method to create a social compose view controller. Do not use any other methods.

