

- Bundle Resources
-  applinks 

Object

# applinks

The root object for a universal links service definition.

iOS 9.0+iPadOS 9.0+macOS 10.15+tvOS 10.0+visionOS 1.0+watchOS 7.0+

``` source
object applinks
```

## Properties

`defaults`

applinks.Defaults

`details`

`[`applinks.Details`]`

`substitutionVariables`

applinks.SubstitutionVariables

## Overview

Use this object to define the universal links you want to associate with your domain.

The object contains these keys:

`defaults`  
The global pattern-matching settings to use as defaults for all universal links in the domain.

`details`  
An array of `Details` objects that define the apps and the universal links they handle for the domain.

`substitutionVariables`  
Custom variables to use for simplifying complex pattern matches. Each name acts as a variable that the system replaces with each string in the associated string array.

Add the JSON code to your `apple-app-site-association` file along with the app identifiers for the apps that you designate to handle universal links for your domain. This example code shows a universal links section in an association file:

```
```

## Topics

### Universal links definitions

object applinks.Details

A list of apps and the universal links they handle for a domain.

### Pattern-matching defaults

object applinks.Defaults

An object that defines the default settings to use for universal links pattern matching.

### Substitution variables

object applinks.SubstitutionVariables

A list of named strings and an associated array of string values that define custom substitution variables to use for URL pattern matching.

