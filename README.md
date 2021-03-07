This is a fork of a project by @jvns.
I needed it for a ctf challenge and thought it would be useful to port it on python 3 and make some improvements to it.
I don't know if I will continue working on it in the future, but if you want to continue this project feel free to do so.

# huffman fun

This hacky Python script prints out the Huffman tree for every block in a gzip file. it may or may not work, no guarantees.

It uses a program called `infgen` available from http://zlib.net/infgen.c.gz.

To try this out on the included gzip file, run

```
$ ./infgen raven.txt.gz | python print_huffman_table.py
```

You should see output like this:


```
' '   : 01100
'a'   : 01101
'e'   : 01110
'i'   : 01111
'n'   : 10000
'o'   : 10001
'r'   : 10010
's'   : 10011
't'   : 10100
'\n'  : 101100
','   : 101101
'b'   : 101110
'c'   : 101111
'd'   : 110000
'f'   : 110001
'h'   : 110010
'l'   : 110011
'm'   : 110100
'p'   : 110101
'u'   : 110110
'g'   : 1110000
'w'   : 1110001
'y'   : 1110010
"'"   : 11101010
'I'   : 11101011
'O'   : 11101100
'S'   : 11101101
'T'   : 11101110
'`'   : 11101111
'k'   : 11110000
'v'   : 11110001
'!'   : 111101010
'-'   : 111101011
'.'   : 111101100
';'   : 111101101
'A'   : 111101110
'B'   : 111101111
'D'   : 111110000
'F'   : 111110001
'G'   : 111110010
'M'   : 111110011
'N'   : 111110100
'P'   : 111110101
'W'   : 111110110
'"'   : 1111110100
'?'   : 1111110101
'C'   : 1111110110
'E'   : 1111110111
'L'   : 1111111000
'q'   : 1111111001
'H'   : 11111110110
'Q'   : 11111110111
'R'   : 11111111000
'j'   : 11111111001
'x'   : 11111111010
```
