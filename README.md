## Sparse Matrix Operations in C++

This C++ program demonstrates operations on sparse matrices using a compressed format that efficiently stores non-zero elements. Sparse matrices are matrices in which most of the elements are zero, and this program saves memory by only storing non-zero elements.

### Classes

1. **`Node` Class**: This class represents individual non-zero elements in the sparse matrix. Each `Node` contains the row, column, and data value of an element. Linked lists of `Node` objects are used to store non-zero elements efficiently.

2. **`sparse_matrix` Class**: This class is used to represent and perform operations on sparse matrices. It includes methods for inserting elements, performing addition and multiplication of sparse matrices, and transposing a matrix. The matrix is represented as a 2D array, with each row containing the row, column, and value of a non-zero element.

### Main Function

The `main` function demonstrates the usage of the `sparse_matrix` class. It performs the following tasks:

- Creates two sparse matrices, inserts elements into them, and allows the user to insert additional elements interactively.
- Performs addition and multiplication of the matrices, and prints the results.
- Computes the transpose of a matrix and prints it.

### Linked Lists

Linked lists are used to efficiently store and access non-zero elements in the sparse matrix. The `create_new_node` function creates a new `Node` and adds it to the linked list, while the `printList` function is used to print the linked list elements.

### Sparse Matrix Operations

- **Addition**: The `add` method of the `sparse_matrix` class performs addition of two sparse matrices. It checks if the matrices have the same dimensions and adds them element-wise, creating a result sparse matrix.

- **Multiplication**: The `multiply` method of the `sparse_matrix` class performs matrix multiplication between two sparse matrices. It checks if the dimensions allow multiplication, transposes one matrix, and then performs the multiplication, creating a result sparse matrix.

- **Transpose**: The `transpose` method of the `sparse_matrix` class computes the transpose of a sparse matrix.

### Interactive User Input

The code allows the user to interactively insert values into either of the two matrices using the console.

This program provides a practical implementation of sparse matrix operations in C++ and demonstrates efficient storage and manipulation of sparse matrices using linked lists.
