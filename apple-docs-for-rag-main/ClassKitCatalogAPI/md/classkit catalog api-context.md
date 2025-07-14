

- ClassKit Catalog API
-  Context 

Dictionary

# Context

An area of your app that represents an assignable task, like a quiz or a chapter.

ClassKit 1.0+

``` source
object Context
```

## Properties

`data`

Context.Data

 (Required) 

The data that makes up the context. This is largely the same information that you provide to the ClassKit framework when you create a CLSContext instance.

`metadata`

Context.Metadata

 (Required) 

Information about the context, like the locale to which the context applies.

## Attributes 

Possible types:

## Mentioned in 

Preparing Context Data

## Discussion

The contexts that you specify in your app as CLSContext instances correspond to the Context.Data object. The Context.Metadata object contains additional information about a context that’s implicit when working with ClassKit in your app.

## Topics

### Objects

object Context.Data

The data that makes up a context.

object Context.Metadata

Information that helps the system categorize a context.

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

object ContextsRequest

A request that you make when modifying context information.

object ContextsResponse

The response you receive after modifying context information.

