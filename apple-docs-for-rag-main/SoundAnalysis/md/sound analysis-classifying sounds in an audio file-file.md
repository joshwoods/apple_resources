

- Sound Analysis
-  Classifying Sounds in an Audio File 

Article

# Classifying Sounds in an Audio File

Identify individual sounds in a file, such as a recording, with an audio file analyzer.

## Overview

Recognize sounds, such as laughter and applause, when they occur in a recording by processing audio files with an SNAudioFileAnalyzer. For example, a sound recording app can use an audio file analyzer to assign searchable metadata tags to each sound file in its library. The same app could also use the analyzer to add timestamps to each recording so that the user can jump to a moment with a specific sound.

### Create a Sound Classification Request

Create an SNClassifySoundRequest by passing a version identifier to the init(classifierIdentifier:) initializer.

```
```

Alternatively, you can create a sound request that uses a custom Core ML model. For example, you can train your own sound classifier with Create ML’s MLSoundClassifier.

Create an SNClassifySoundRequest with a custom sound classifier model:

1.  Add a sound classifier’s Core ML model file to your project (see Integrating a Core ML Model into Your App).

2.  Create an instance of the model’s wrapper class. Xcode automatically generates a class with the same name (minus the `mlmodel` extension).

3.  Pass the instance’s `model` property to the init(mlModel:) initializer.

```
```

### Implement a Results Observer

Implement a type that receives results from an audio analyzer by adopting the SNResultsObserving protocol. The protocol defines the methods an analyzer calls as it generates results or errors, or when it completes a task.

```
```

The observer in this example prints the prediction’s result — a timestamp, a classification name, and the classifier’s confidence — to the console. Implement your observer to take action that’s appropriate for your app according to the result.

Important

You must maintain a strong reference to your observer. Sound analyzers don’t keep strong references to your observer.

### Create an Audio File Analyzer

Analyze an audio file by creating an SNAudioFileAnalyzer and passing a URL to an audio file to the init(url:) initializer.

```
```

Tip

Audio file analyzers work with any compressed or uncompressed audio file format that Core Audio supports.

Add your sound classification request and results observer to the analyzer by calling the add(_:withObserver:) method.

```
```

Start analyzing the audio file by calling the analyze() or analyze(completionHandler:) methods.

```
```

### Receive the Results

The audio analyzer sends each result to your SNResultsObserving instance as it processes the audio data.

```
Analysis result for audio at time: 1.45
Acoustic Guitar: 92.39% confidence.

...

Analysis result for audio at time: 8.74
Acoustic Guitar: 94.45% confidence.

...

Analysis result for audio at time: 14.15
Tambourine: 85.39% confidence.

...

Analysis result for audio at time: 20.92
Snare Drum: 96.87% confidence.
```

## See Also

### Audio analyzers

class SNAudioFileAnalyzer

An analyzer that runs sound classification requests on an audio file.

Classifying Sounds in an Audio Stream

Identify individual sounds in an audio data stream, such as from a microphone, with an audio stream analyzer.

class SNAudioStreamAnalyzer

An object you create to analyze a stream of audio data and provide the results to your app.

