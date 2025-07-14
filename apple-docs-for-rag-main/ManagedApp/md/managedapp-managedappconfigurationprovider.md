

- ManagedApp
-  ManagedAppConfigurationProvider 

Class

# ManagedAppConfigurationProvider

A class that provides configurations that an MDM admin provisions for a managed app or extension.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
class ManagedAppConfigurationProvider
```

## Overview

This class provides objects of a type you define, which decodes and validates the configuration that the framework receives from the MDM server.

The framework ingests the configuration in the form of a property list that the MDM server provides and passes to your type as a Decoder. Your type conforms to Decodable and parses the configuration according to your specification that the server admin conforms to when creating the property list.

If the decoder encounters a problem, it throws an error that the MDM admin can find in the device’s event log.

## Topics

### Initializing a configuration provider

init()

Initializes a configuration provider.

### Accessing configurations

func configurations&lt;Configuration>(Configuration.Type) async -> some AsyncSequence&lt;Optional&lt;Configuration>, Never> 

Provides an asynchronous sequence of configurations that the MDM admin specifies.

## See Also

### Configuration

Specifying and decoding a configuration

Publish a configuration specification and implement a decoder that parses and validates configuration provided by an MDM admin.

