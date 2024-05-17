**Huffman File Compression**

**Overview**
This Python program implements Huffman's algorithm for file compression. Huffman's algorithm is a widely used method for lossless data compression. It works by assigning variable-length codes to input characters based on their frequencies, with the goal of minimizing the total number of bits required to represent the input data.

**DSA Strategies used:**

**1. Hash Table (Frequency Counting):**
Before constructing the Huffman tree, the program needs to count the frequencies of characters in the input file. To efficiently store and update the frequency counts, a hash table (dictionary in Python) is often used.
The program utilizes a hash table to count the frequencies of characters in the input file, facilitating the subsequent construction of the Huffman tree.

**2. Binary Tree (Huffman Tree):**
Huffman's algorithm constructs a binary tree where each leaf node represents a character and each internal node represents the merge of two nodes. The binary tree is built in such a way that characters with higher frequencies are closer to the root, resulting in shorter codes. The program creates and traverses the Huffman tree to assign variable-length codes to characters based on their frequencies. The tree is typically implemented using a data structure such as a binary tree or a linked list.

**3. Priority Queue (Min Heap):**
Huffman's algorithm requires efficient access to the characters with the lowest frequencies during tree construction. This is typically implemented using a priority queue, with characters sorted by their frequencies (lowest frequency characters have the highest priority).
In the program, a min heap priority queue is often used to efficiently select and merge the nodes with the lowest frequencies during the construction of the Huffman tree.

**4. Greedy Algorithm:**
Huffman's algorithm is a greedy algorithm, as it makes locally optimal choices at each step (merging the two nodes with the lowest frequencies) to achieve a globally optimal solution (minimal total encoding length).
The program iteratively selects and merges nodes with the lowest frequencies until a single root node is obtained, forming the Huffman tree. This greedy approach ensures an efficient encoding scheme.

**Features**
1. Compresses input files using Huffman's algorithm.
2. Decompresses previously compressed files.
3. Efficiently handles both text and binary files.
4. Provides options for specifying input and output file paths.

**Usage**
1. Installation - Clone the repository or download the source code.
2. Ensure you have Python installed on your system (version 3.x).
3. Install the required dependencies by running:
4. Run the program
5. Give the file, which you want to compress
6. you will get compressed file
7. Likewise, you can decompress the file and get the uncompressed file as well
