# 📦 ZipX – File Compression using Huffman Encoding

This C++ project implements **lossless data compression and decompression** using the Huffman encoding algorithm. It compresses text files into `.huf` format and decompresses them back to original form with high efficiency.

---

## 🧠 Overview

Huffman encoding assigns **shorter binary codes** to more frequent characters and longer codes to rare ones. This ensures maximum compression with zero data loss.

---

## 🧩 Procedure

### 🔐 Compression

1. **Frequency Calculation** – Scans `inputFile.txt` and counts character frequencies.
2. **Huffman Tree Construction** – Builds a tree using a min-heap based on frequency.
3. **Code Generation** – Traverses the tree to assign binary codes to each character.
4. **Encoding** – Replaces each character with its Huffman code.
5. **Output** – Encoded data is written to `compressionFile.huf`.

### 🔓 Decompression

1. **Read Huffman Tree & Encoded Data** – From `compressionFile.huf`.
2. **Reconstruct Huffman Tree** – Using the stored metadata.
3. **Decoding** – Uses tree traversal to decode binary back into characters.
4. **Output** – Restores original text into `outputFile.txt`.

---

## 🛠️ Compilation Instructions

### ✅ Compress

```bash
g++ encode.cpp huffman.cpp -o main
./main inputFile.txt compressionFile.huf
