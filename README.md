## Compression tool using Huffman Encoding in GO

### How to use:

```bash

go build

./compression_tool_huffman
Usage of ./compression_tool_huffman:
  -d    If set, input file will be decompressed to the output file
  -f string
        The name of the input file to be compressed
  -o string
        The name of the output compressed file
```


### Compress a file:
```bash
 ls -lh test_text.txt test_compressed.txt                                                                                 
-rw-rw-r-- 1 jitesh jitesh 1.8M Jul  9 19:10 test_compressed.txt
-rw-r--r-- 1 jitesh jitesh 3.2M Jul  9 12:31 test_text.txt

```
### Decompress a file:

```bash
./compression_tool_huffman -f test_compressed.txt -o original.txt -d                                                    
 ls -lh *.txt                                                                                                             
-rw-rw-r-- 1 jitesh jitesh 3.2M Jul  9 19:12 original.txt
-rw-rw-r-- 1 jitesh jitesh 1.8M Jul  9 19:10 test_compressed.txt
-rw-r--r-- 1 jitesh jitesh 3.2M Jul  9 12:31 test_text.txt

```
