---
description: Basic description of problems with OP_CAT
---

# 😿 OP\_CAT Problem

In the context of Bitcoin Script, there are multiple operating codes (opcodes), each of which performs certain operations in the virtual machine.

However, despite the variety of possibilities, some opcodes were criticized and excluded from the protocol. Among them is OP\_CAT, which represented a data string concatenation operation and has a rich history in the development of Bitcoin as a whole.

***

### Performance

OP\_CAT could cause performance issues due to inefficiencies in implementation. String concatenation can be a resource-intensive operation, resulting in additional overhead for smart contract execution and transaction processing.

### Ambiguity of use

The application of string concatenation in the context of smart contracts can often be unclear and lead to unexpected results. This complicates code analysis and verification, and makes it harder to predict its behavior.

### Security and vulnerabilities.

One of the main concerns that led to the abandonment of OP\_CAT was the potential security risks. The concatenation operation can be a source of vulnerabilities such as buffer overflows if proper precautions are not taken.

***

OP\_CAT was originally included in early versions of Bitcoin, but was removed in 2010 due to concerns about various problems. However, as technology has evolved and understanding has increased, these concerns have been addressed. The reconsideration of the decision to include OP\_CAT is becoming an important development. It is not just about going back in time, it is about opening up new perspectives to create scenarios in the context of bitcoin.
