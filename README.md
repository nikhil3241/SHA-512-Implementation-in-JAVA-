# SHA-512-Implementation-in-JAVA-

SHA-512 is a hashing algorithm that performs a hashing function on some data given to it.
Hashing algorithms are used in many things such as internet security, digital certificates and even blockchains. Since hashing algorithms play such a vital role in digital security and cryptography, this is an easy-to-understand walkthrough, with some basic and simple maths along with some diagrams, for a hashing algorithm called SHA-512. It’s part of a group of hashing algorithms called SHA-2 which includes SHA-256 as well which is used in the bitcoin blockchain for hashing.

Hashing Functions - 
Hashing functions take some data as input and produce an output (called hash digest) of fixed length for that input data. This output should, however, satisfy some conditions to be useful.
1. Uniform distribution: Since the length of the output hash digest is of a fixed length and the input size may vary, it is apparent that there are going to be some output values that can be obtained for different input values. Even though this is the case, the hash function should be such that for any input value, each possible output value should be equally likely. That is to say that every possible output has the same likelihood to be produced for any given input value.
2. Fixed Length: This is should be quite self-explanatory. The output values should all be of a fixed length. So, for example, a hashing function could have an output size of 20  characters or 12 characters, etc. SHA-512 has an output size of 512 bits.
3. Collision resistance: Simply speaking, this means that there aren’t any or rather it is not feasible to find two distinct inputs to the hash function that result in the same output (hash digest).

