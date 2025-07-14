

- ClassKit Catalog API
-  ContextsRequest 

Dictionary

# ContextsRequest

A request that you make when modifying context information.

ClassKit 1.0+

``` source
object ContextsRequest
```

## Properties

`contexts`

`[`Context`]`

 (Required) 

An array of contexts that can contain up to 200 context objects.

## Attributes 

Possible types:

## Discussion

Use this request object to define one or more contexts that your app provides.

## See Also

### Declaring Contexts

Preparing Context Data

Adjust how you manage context data when working with the web API.

Create or Replace Contexts

Store information about the assignable content that your educational app provides.

Get a Context

Fetch information that you previously stored about your app’s assignable activities.

Delete a Context

Remove information that you previously stored about your app’s assignable activities.

object Context

An area of your app that represents an assignable task, like a quiz or a chapter.

object ContextsResponse

The response you receive after modifying context information.

