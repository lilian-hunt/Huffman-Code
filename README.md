# Huffman-Code
Huffman code is a set of encoding designed to minimized the size of the message, by reducing the size of characters which are frequently used.  In Huffman code, each character can have a different number of bits similar to Morse code, but unlike ASCII, where each character are of a fixed size.  The code is constructed by creating a binary tree of each character as follows:

Count the frequency of each letter in the message

For each letter, construct a leaf node containing the letter and the frequency

While there are more than one node remaining, combine the two nodes with the smallest frequency into a new node with the combined frequency

If there are more than one nodes with the same frequency, choose the node which contains the letter with the smallest ASCII value, i.e, use the ASCII value of the smallest letter within the node

Once the tree is constructed, the code can be read by traversing the tree.  If we denote travelling along a branch with the higher frequency as 0 and along lower frequency with 1, then trvallening to the letter t on the tree below gives a path of 0100.

The program asks the user for a message to encode,  then prints the code from the letter to binary (orderd by the binary code) and the encoded message.
