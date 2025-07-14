

- Metal
- Shader Libraries
- Metal Libraries
-  Building a Shader Library by Precompiling Source Files 

Article

# Building a Shader Library by Precompiling Source Files

Create a shader library that you can add to an Xcode project with the Metal compiler tools in a command-line environment.

## Overview

Manually compile your Metal Shading Language (MSL) source files into a Metal shader library outside of an Xcode project with the Metal command-line tools. The `metal` compiler tool converts each shader source file into an intermediate representation file. The `metallib` and `metal-ar` tools then compile intermediate representation files into a library and a binary archive, respectively.

You can create a library from one or more intermediate representation files, one or more archive files, or a combination of both.

### Compile a Shader Source File into a Library

The simplest way to compile and build a single MSL source file into a library file is with two commands. The first command invokes the `metal` compiler tool, which compiles the source file into an intermediate representation file.

```
% xcrun -sdk macosx metal -o Shadow.ir  -c Shadow.metal
% xcrun -sdk macosx metal -o PointLights.ir  -c PointLights.metal
% xcrun -sdk macosx metal -o DirectionalLight.ir  -c DirectionalLight.metal
```

The `-o` option indicates the output file name and the `-c` option tells the tool to preprocess, compile, and assemble the source file.

Note

This example uses the `macosx` SDK, but you can use any SDK your app targets.

Optionally, you can combine several intermediate representation files into a single Metal archive with the `metal-ar` tool.

```
% xcrun -sdk macosx metal-ar -q Lights.metalar DirectionalLight.ir PointLights.ir
```

The `-q` option tells the tool to quickly append to its argument, which creates a new archive file if it doesn’t already exist.

Build a Metal library from one or more intermediate representation files, one or more archive files, or a combination of both with the `metallib` command.

```
% xcrun -sdk macosx metallib -o LightsAndShadow.metallib Lights.metalar Shadow.ir
```

The command produces a Metal library that your app can load at runtime. One way to do this is by adding it to your project’s build targets in Xcode.

Note

The Metal command-line tools for Windows use the same options and arguments as their macOS counterparts.

### Retrieve and Load a Library

At runtime, you can access a library by creating an MTLLibrary instance with the makeLibrary(URL:) method.

- Swift
- Objective-C

```
func createLibrary(_ device: MTLDevice, libraryName: String) -> MTLLibrary? {
    let libraryURL = Bundle.main.url(forResource: libraryName,
                                     withExtension: "metallib")

    guard let libraryURL else {
        print("Couldn't find library file: \(libraryName)");
        return nil;
    }

    let library: MTLLibrary
    do {
        library = try device.makeLibrary(URL: libraryURL)
    } catch {
        print("Couldn't find library file: \(libraryName)");
        print("Error descriotion: \(error.localizedDescription)")
        return nil
    }

    return library
}
```

```
+ (id) createLibrary:(id)device
                        fromName:(NSString*)libraryName
{
    NSURL *libraryURL = [[NSBundle mainBundle] URLForResource:libraryName
                                                withExtension:@"metallib"];

    if (libraryURL == nil) {
        NSLog(@"Couldn't find library file: %@", libraryName);
        return nil;
    }

    NSError *libraryError = nil;
    id  library = [device newLibraryWithURL:libraryURL
                                                  error:&libraryError];
    if (library == nil) {
        NSLog(@"Couldn't create library: %@", libraryName);

        if (description != nil) {
            NSLog(@"Error description: %@", libraryError.localizedDescription);
        }
        return nil;
    }

    return library;
}
```

## See Also

### Working with Metal Intermediate Representation Libraries

Minimizing the Binary Size of a Shader Library

Reduce the storage footprint of your shaders, and potentially reduce their compile time, by selecting the Metal compiler’s size optimization option.

Generating and Loading a Metal Library Symbol File

Debug your Metal shaders from your production apps by creating companion symbol files at compile time and loading them at debug time.

