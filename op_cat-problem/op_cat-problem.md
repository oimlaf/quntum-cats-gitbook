---
description: Description of problems with OP_CAT
---

# 😿 OP\_CAT Problem

In the context of Bitcoin Script, there are several opcodes (opcodes), each of which performs certain operations in the virtual machine. However, despite the variety of possibilities, some opcodes have been criticized and excluded from the protocol.

One of these is OP\_CAT, which took its place among opcodes. However, it was removed in 2010 due to concerns about its potential to contribute to scripts with exponentially increasing memory usage proportional to the size of the script, as well as a host of other implicit problems, which are described below.

#### Performance

OP\_CAT could cause performance issues due to inefficiencies in implementation. String concatenation can be a resource-intensive operation, resulting in additional overhead for smart contract execution and transaction processing.

#### Ambiguity of use

The application of string concatenation in the context of smart contracts can often be unclear and lead to unexpected results. This complicates code analysis and verification, and makes it harder to predict its behavior.

#### Security and vulnerabilities.

One of the main concerns that led to the abandonment of OP\_CAT was the potential security risks. The concatenation operation can be a source of vulnerabilities such as buffer overflows if proper precautions are not taken.



But things have changed over time, and many are now reassessing the threats associated with the use of OP\_CAT, which has spawned the idea of bringing it back

***
