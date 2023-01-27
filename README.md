# Neural-Cryptography

A neural network is a series of algorithms that endeavors to recognize underlying relationships in a set of data through a process that mimics the way the human brain operates. Encryption is the process of establishing a secure connection such that only authorized parties can understand the information. Cryptography is the study of secure communications techniques that allow only the sender and intended recipient of the message to view its content. Neural cryptography is a branch of cryptography that analyzes the application of stochastic algorithms, especially artificial neural network algorithms for use in encryption and cryptanalysis.

Neural networks can learn to protect the confidentiality of their data from other neural networks, they discover forms of encryption and decryption without being taught specific algorithms for these purposes. In this project we involve three parties. They are Alice, Bob and Eve. Alice and Bob wish to communicate securely and Eve wishes to eavesdrop on their communication. After a bit of training, Eve may start to break this code. With some more training, Alice and Bob discover refinements, in particular codes that exploit the key material better. Eve eventually finds it impossible to adjust to those codes.

Eve’s goal is to reconstruct the message accurately, in other words, to minimize the error between message sent by Alice and message received by Eve.

Alice and Bob want to communicate clearly (to minimize the error between message sent by Alice and message received by Bob), but also to hide their communication from Eve.

A more realistic and useful goal for Alice and Bob is, generally, to minimize the mutual information between Eve’s guess and the real message.

## Block Diagram:
![image](https://user-images.githubusercontent.com/67183417/215109649-0ee0c638-feb2-4a58-9d36-632b0dd9fb86.png)

Initialization and Pre-Processing Block handles preliminary tasks like setting the parameters for the other processes and blocks to operate on.

Encryption Block contains three key components namely, Plaintext (P) which is the input, the Key (K) which is received from the previous block and the sender Alice. When Alice sends the Plaintext, it is encrypted using the key and sent as an encrypted message called the Ciphertext (C)

Decryption Block consists of the receiver of the encrypted message, i.e., the Ciphertext, who we call Bob in this scenario. Bob receives the key from the previous block and using the key, he is able to decrypt the message back to Plaintext.

Fourth optional block is called the Man-in-the-Middle Block consisting of Eve who is privy to the Ciphertext and is an unauthorized middle man who is not supposed to have access to the data. Using techniques like Brute Force and other algorithms to find the key, Eve could gain access from the Encryption Block in an unsolicited manner and find out the Plaintext.
