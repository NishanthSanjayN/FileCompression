# File-compression-using-Huffman-encoding

## Overview
This C++ project implements Huffman encoding, a popular technique for lossless data compression and decompression. Huffman encoding efficiently reduces the size of files by assigning variable-length codes to different characters based on their frequencies within the input data.

## Procedure
### Compression
1. **Frequency Calculation**: The program scans the input file to calculate the frequency of each character present.
2. **Building the Huffman Tree**: Using the character frequencies, a Huffman tree is constructed, where characters with higher frequencies are assigned shorter codes.
3. **Generating Huffman Codes**: Traversing the Huffman tree, unique codes are assigned to each character.
4. **Encoding**: The input file is then read again, and each character is replaced with its respective Huffman code, effectively compressing the data.
5. **Output**: The compressed data is written into an output file.

### Decompression
1. **Reading Huffman Tree**: The compressed file contains the Huffman tree information and the encoded data.
2. **Reconstructing Huffman Tree**: Using the tree information in the compressed file, the Huffman tree is reconstructed.
3. **Decoding**: The encoded data is read, and using the Huffman tree, it's decoded back to its original form.
4. **Output**: The decoded data is written into an output file.
   ![image](https://github.com/JanviBagrecha/File-compression-using-Huffman-encoding/assets/111588269/0aa47912-6380-4f9c-8c7b-b95761bc3564)

## Usage
1. Compile the C++ program using your preferred compiler.
2. Run the executable file providing the input file path for compression or the compressed file path for decompression.
3. Check the output file for the compressed or decompressed data respectively.

## Support or Contact
For any inquiries or support regarding the Huffman Encoding and Decoding project, please contact janvi.bagrecha@gmail.com.
