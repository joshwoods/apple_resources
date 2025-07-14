

- PHASE
-  PHASEAssetRegistry 

Class

# PHASEAssetRegistry

A central repository of audio assets.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEAssetRegistry
```

## Overview

This class manages audio by registering two types of assets throughout the app’s life cycle:

PHASESoundAsset  
A sound asset identifies the particular audio data that your app intends to play.

PHASESoundEventNodeAsset  
A sound event asset provides audio with an avenue to the output device, and either represents a single sound or a dynamic set of sounds that play individually, depending on the app’s state.

When you’re done with a sound asset, call unregisterAsset(identifier:completion:) to free up its system resources.

## Topics

### Registering Sound Assets

Load shared audio data that your app can access and play from any scope.

func registerSoundAsset(url: URL, identifier: String?, assetType: PHASEAsset.AssetType, channelLayout: AVAudioChannelLayout?, normalizationMode: PHASENormalizationMode) throws -> PHASESoundAsset

Loads a sound asset from the argument URL and adds it to the engine’s list of registered assets.

func registerSoundAsset(data: Data, identifier: String?, format: AVAudioFormat, normalizationMode: PHASENormalizationMode) throws -> PHASESoundAsset

Loads a sound asset from memory and adds it to the engine’s list of registered assets.

func unregisterAsset(identifier: String, completion: ((Bool) -> Void)?)

Deallocates system memory for a given asset and removes it from the engine’s list of registered assets.

### Registering Sound Event Assets

Define playback objects that your app invokes for one-time audio output, or a sophisticated hierarchy that varies the output based on your app’s state.

func registerSoundEventAsset(rootNode: PHASESoundEventNodeDefinition, identifier: String?) throws -> PHASESoundEventNodeAsset

Registers the root node of the sound event asset.

func asset(forIdentifier: String) -> PHASEAsset?

Provides the asset named with the designated identifier.

### Registering Global Metaparameters

Centralize audio parameters that change the charactaristics of in-flight audio, and synchronize across multiple playback events.

func registerGlobalMetaParameter(metaParameterDefinition: PHASEMetaParameterDefinition) throws -> PHASEGlobalMetaParameterAsset

Registers a global metaparameter with the asset registry.

var globalMetaParameters: [String : PHASEMetaParameter]

A dictionary of metaparameters that all sound event assets share.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Setup

class PHASEEngine

An object that manages audio assets, controls playback, and configures environmental effects.

enum UpdateMode

Modes that determine when the framework consumes API calls and updates internal state.

enum PHASENormalizationMode

Options that determine whether the framework adjusts a sound asset’s loudness for the user’s output device.

enum PHASESpatializationMode

The manner in which PHASE outputs spatial audio.

enum PHASEReverbPreset

The manner in which PHASE diffuses resonating sound.

class PHASEMedium

A property or quality of the environment that affects how sound travels.

