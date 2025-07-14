

- Installer JS
-  Choice 

# Choice

A single installation choice.

## Overview

Choice objects are properties of the `choices` global variable and represent the installation choices defined in a distribution package.

The name of each property of the `choices` array corresponds to the `choice-id` attribute of each of the distribution’s installation choices (see Distribution Definition XML Schema Reference for more information). Therefore, a specific choice is accessed this way:

choices.&lt;choice-id>

`` represents the identifier of the desired choice in the installation definition. For example, to access the `selected` property of a choice with `'choice_a'` as its identifier, you would use the following expression:

choices.[&#39;choice_a&#39;].selected

## Topics

### Accessing a Choice’s State

selected

A Boolean value that indicates whether the choice is selected.

enabled

A Boolean value that indicates whether the choice is enabled.

visible

A Boolean that indicates whether the choice is visible.

### Accessing a Choice’s Metadata

title

The title of the distribution package, as a String.

description

The description of the distribution, as a String.

### Working with Packages

packages

An array identifying each package attached to the choice.

packageUpgradeAction

A string specifying the relationship between the choice’s packages (specified by the packages property) and the same packages (based on the package identifier) installed on the host.

