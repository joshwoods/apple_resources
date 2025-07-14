

- Metal Performance Shaders
-  Matrices and Vectors 

API Collection

# Matrices and Vectors

Solve systems of equations, factorize matrices and multiply matrices and vectors.

## Topics

### Matrices

class MPSMatrix

A 2D array of data that stores the data's values.

class MPSMatrixDescriptor

A description of attributes used to create an MPS matrix.

class MPSTemporaryMatrix

A matrix allocated on GPU private memory.

### Vectors

class MPSVector

A 1D array of data that stores the data's values.

class MPSVectorDescriptor

A description of the length and data type of a vector.

class MPSTemporaryVector

A vector allocated on GPU private memory.

### Classes for Decomposition and Solving

class MPSMatrixDecompositionCholesky

A kernel for computing the Cholesky factorization of a matrix.

class MPSMatrixSolveCholesky

A kernel for computing the solution of a linear system of equations using a Cholesky factorization.

class MPSMatrixDecompositionLU

A kernel for computing the LU factorization of a matrix using partial pivoting with row interchanges.

class MPSMatrixSolveLU

A kernel for computing the solution of a linear system of equations using an LU factorization.

class MPSMatrixSolveTriangular

A kernel for computing the solution of a linear system of equations using a triangular coefficient matrix.

class MPSMatrixUnaryKernel

A kernel that consumes one matrix and produces one matrix.

class MPSMatrixBinaryKernel

A kernel that consumes two matrices and produces one matrix.

enum MPSMatrixDecompositionStatus

### Matrix Arithmetic Operations

class MPSMatrixSum

A kernel for performing a pointwise summation of a matrix.

class MPSMatrixMultiplication

A matrix multiplication kernel.

class MPSMatrixVectorMultiplication

A matrix-vector multiplication kernel

class MPSMatrixFindTopK

A kernel for computing the top-K values and their corresponding indices in a matrix.

### Matrix Copying Operations

class MPSMatrixCopy

A class that can perform multiple matrix copy operations.

class MPSMatrixCopyToImage

A kernel that copies matrix data to a Metal Performance Shaders image.

class MPSMatrixCopyDescriptor

A description of multiple matrix copy operations.

class MPSImageCopyToMatrix

A class that copies image data to a matrix.

### Matrix Neural Network Operations

class MPSMatrixFullyConnected

A kernel for applying a fully connected neural network layer.

class MPSMatrixFullyConnectedGradient

A kernel for applying a fully gradient connected neural network layer.

class MPSMatrixNeuron

A neuron activation kernel that operates on matrices.

class MPSMatrixNeuronGradient

A gradient neuron activation kernel that operates on matrices.

### Matrix Softmax Operations

class MPSMatrixLogSoftMax

A logarithmic softmax kernel that operates on matrices.

class MPSMatrixLogSoftMaxGradient

A logarithmic gradient softmax kernel that operates on matrices.

class MPSMatrixSoftMax

A softmax kernel that operates on matrices.

class MPSMatrixSoftMaxGradient

A gradient softmax kernel that operates on matrices.

### Matrix Normalization Operations

class MPSMatrixBatchNormalization

A batch normalization kernel that operates on matrices.

class MPSMatrixBatchNormalizationGradient

A batch normalization gradient kernel that operates on matrices.

