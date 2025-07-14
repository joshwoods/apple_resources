

- AVFAudio
-  Speech synthesis 

API Collection

# Speech synthesis

Configure voices to speak strings of text.

## Overview

The Speech Synthesis framework manages voice and speech synthesis, and requires two primary tasks:

Create an AVSpeechUtterance instance that contains the text to speak. Optionally, configure speech parameters, such as voice and rate, for each utterance.

```
// Create an utterance.
let utterance = AVSpeechUtterance(string: "The quick brown fox jumped over the lazy dog.")

// Configure the utterance.
utterance.rate = 0.57
utterance.pitchMultiplier = 0.8
utterance.postUtteranceDelay = 0.2
utterance.volume = 0.8

// Retrieve the British English voice.
let voice = AVSpeechSynthesisVoice(language: "en-GB")

// Assign the voice to the utterance.
utterance.voice = voice
```

Pass the utterance to an AVSpeechSynthesizer instance to produce spoken audio.

```
// Create a speech synthesizer.
let synthesizer = AVSpeechSynthesizer()

// Tell the synthesizer to speak the utterance.
synthesizer.speak(utterance)
```

Optionally, use the speech synthesizer instance to control or respond to ongoing speech; for example, assign its delegate to receive speech event notifications.

## Topics

### Spoken text attributes

class AVSpeechUtterance

An object that encapsulates the text for speech synthesis and parameters that affect the speech.

class AVSpeechSynthesisVoice

A distinct voice for use in speech synthesis.

### Speech synthesis controls

class AVSpeechSynthesizer

An object that produces synthesized speech from text utterances and enables monitoring or controlling of ongoing speech.

### Speech synthesis audio unit

class AVSpeechSynthesisProviderAudioUnit

An object that generates speech from text.

