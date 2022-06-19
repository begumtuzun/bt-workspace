# bt-workspace
Homomorphic encryption is a type of encryption that enables particular
computations on ciphertexts to produce an encrypted result that, when
decrypted, is identical to the outcome of operations carried out on the
plaintexts.

Graph theory is the study of graphs, which are mathematical structures
used to model relationships between objects. In cybersecurity, a
graph-based approach centers on preserving the context of security
events. By structuring an organization's historical incident data as a
graph, security operations teams can preserve and visualize
relationships across all of the data elements.

In this study is it aimed to implement a selected graph algorithm which
is \"all paths from source to a destination\" in a privacy-preserving
manner using homomorphic encryption (Microsoft EVA).

# Introduction

In this report, we aim to implement a graph algorithm "all paths from
source to a destination\" in a privacy-preserving manner using
homomorphic encryption.

The term homomorphism is derived from the Greek words homos, which means
\"same,\" and morphe, which means \"shape.\" In computer science,
homomorphic encryption is used to convert plaintext to ciphertext.
Plaintext is any data that a sender wishes to send to a receiver. It can
be viewed as the input to any algorithm or as information being
transmitted prior to encryption by an algorithm. Email messages, word
processor files, images, and ATM and credit card transaction information
are all examples of plaintext. This plaintext is converted to
ciphertext, which is encrypted data that is unreadable until decrypted
with a key.

# Background

## Homomorphic Encryption

Homomorphic encryption allows you to analyze or manipulate encrypted
data without disclosing it to anyone. Homomorphic encryption is a type
of encryption that allows users to compute on encrypted data without
first decrypting it. These resulting computations are left in encrypted
form, which when decrypted produces the same output as if the operations
had been performed on unencrypted data. Homomorphic encryption can be
used to ensure the privacy of outsourced storage and computation. This
enables data to be encrypted before being sent to commercial cloud
environments for processing.

## Selected Graph Algorithm: All Paths From A Given Source to A Destination 

This algorithm finds all paths from the source node to the destination
node by checking every single connection with nodes. More in detail, it
starts with checking all edges from the source node to all its
neighbors. In the next step, "the neighbor node" will be the new "source
node" and the algorithm checks its neighbors. This loop continues until
the algorithm reaches the destination node. In the end, it prints the
list of the paths from the first source node to the destination node.

## Microsoft EVA

EVA is a homomorphic encryption compiler that automates the parts that
require cryptographic expertise. This allows you to write programs that
operate on encrypted data without knowing the secret key. Consider EVA
to be the homomorphic world's \"C compiler.\" EVA IR (Encrypted Vector
Arithmetic Intermediate Representation) homomorphic computations are
compiled to the homomorphic encryption library API's \"assembly.\" EVA,
like C compilers, frees you from difficult tasks like register
allocation and encryption parameter selection, rescaling insertion, and
relinearization.

# Implementation

Project has a graph in the function of "simulate" which has a variable
of inputs that comes from prepareInput, which type of a list. This list
keeps connections among all nodes as a single matrix in it. When we
implement the print algorithm, we used this list. We divided this list
according to the given n, which is node count, and therefore, we
transformed this list into a 2 dimensions matrix. Furthermore, we
transformed the last list as parameters of the findpaths function. In
the end, we sent the last list to the findpath function and we obtain
all paths which are from the source to the destination. As a result, we
found all paths by selecting a certain nodecount value, and then we made
the destination node equal to the nodecount value. Finally, we printed
all paths with a loop from source node value to destination node value
by increasing 1 the source node value.

## Creation of Nodes and Graphs

NetworkX was used to create a random graph. NetworkX is a Python package
for creating, manipulating, and studying complex networks' structure,
dynamics, and functions. After creating a random graph selected graph
algorithm was implemented.

Diffferent graph structures are given below.

![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/plotgraph36smcnt0.png)
![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/plotgraph32smcnt0.png)
![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/plotgraph40smcnt0.png)

## Implementation Findings

Results according to simcnt value are shown in the tables below.

![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/res0.PNG)
![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/res1.PNG)
![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/res2.PNG)

# Results

![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/result0.png)
![image](https://github.com/begumtuzun/bt-workspace/blob/master/Images/result2.png)

# Conclusion

Homomorphic Encryption is one of the most important types of encryption
methods being researched in computational sciences today. It is
significant because all of the techniques, including fully, somewhat,
and partially homomorphic encryption, allow for the secure transmission,
storage, and processing of encrypted data without jeopardizing the
information's confidentiality. The success of its application can be
seen in a variety of industries, including finance and medicine.
Researchers have benefited from incorporating homomorphic encryption
research into their own work and will continue to excel in its
application in the future.
