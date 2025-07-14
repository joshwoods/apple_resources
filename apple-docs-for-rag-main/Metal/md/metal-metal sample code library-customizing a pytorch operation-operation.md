

- Metal
- Metal Sample Code Library
-  Customizing a PyTorch operation 

Sample Code

# Customizing a PyTorch operation

Implement a custom operation in PyTorch that uses Metal kernels to improve performance.

Download

## Overview

Note

This sample code project is associated with WWDC23 session 10050: Optimize machine learning for Metal apps.

### Configure the sample code project

Before you run the sample code project:

1.  Follow the instructions in Accelerated PyTorch training on Mac.

2.  Install PyTorch nightly (Python 3.7 or later is required).

    ```
    pip3 install --pre torch --index-url https://download.pytorch.org/whl/nightly/cpu
    ```

3.  Install Ninja

    ```
    pip3 install Ninja
    ```

4.  Run the sample.

    ```
    python3 run_sample.py
    ```

## See Also

### Compute Workflows

Performing Calculations on a GPU

Use Metal to find GPUs and perform calculations on them.

Selecting Device Objects for Compute Processing

Switch dynamically between multiple GPUs to efficiently execute a compute-intensive simulation.

Customizing a TensorFlow operation

Implement a custom operation that uses Metal kernels to accelerate neural-network training performance.

