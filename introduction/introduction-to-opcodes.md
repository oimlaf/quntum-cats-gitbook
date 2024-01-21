---
description: Basic definition of Opcodes
---

# 📖 Introduction to Opcodes

Opcodes are a set of instructions in the Bitcoin Script virtual machine, which is used to write smart contracts, and also serve as the basic building blocks of transaction execution scripts to determine what conditions must be met for funds to be spent.

{% hint style="info" %}
Bitcoin Script is a small and limited programming language that is embedded in Bitcoin transactions to define conditions and rules for their execution.
{% endhint %}

{% hint style="info" %}
BitVM (Bitcoin Virtual Machine) - a proposed system for verifying bitcoin calculations and transactions.
{% endhint %}

Bitcoin Script is designed to provide a more flexible use of funds than simply transferring bitcoins. It provides the ability to set different conditions under which funds can be spent, depending on the fulfillment of certain script conditions.

Opcodes can be divided into two main categories: standard (also known as "restricted") and non-standard (or "unpredictable"). Standard opcodes are supported by all full nodes in the Bitcoin network, while non-standard opcodes may only be supported by some nodes or not at all.

Examples of standard opcodes include OP\_CHECKSIG, which verifies the transaction signature, and OP\_IF, which branches script execution based on conditions.

More interesting are the non-standard opcodes. It is important to note that many of them can change and evolve with the development of the Bitcoin protocol. Below are examples of non-standard opcodes that may have been used at different points in time:

* **OP\_VER -** is designed to version scripts and support future changes. Disabled due to potential security threats;
* **OP\_CAT и OP\_SPLIT -** are intended for string concatenation (concatenation) and string separation. Disabled due to performance and potential security risks;
* **OP\_EVAL -** allows executing arbitrary scripts inside the current script. Disabled due to potential security risks;
* **OP\_XOR -** performs an exclusive OR operation on the bytes in the stack. Disabled due to potential security threats.

Bitcoin's opcode system is an integral part of its functionality, providing a toolkit for creating a variety of transaction scenarios, ensuring the flexibility and security of the network. Understanding their functionality is of key importance to developers, users, and everyone who interacts with this system. The evolution of opcodes reflects the dynamics of Bitcoin, and keeping up with these changes is essential to staying current in the use of the cryptocurrency.
