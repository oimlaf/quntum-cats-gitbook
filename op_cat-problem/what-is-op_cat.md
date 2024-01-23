---
description: Definition of OP_CAT
---

# 🐈 What is OP\_CAT?

As sad as it may sound, the acronym OP\_CAT has nothing to do with the kitties we all love so much. OP\_CAT stands for Operation Code Concatenate, and it is an opcode used for concatenation, i.e. concatenating (combining) data.

{% hint style="info" %}
OP\_CAT is an opcode for data concatenation
{% endhint %}

***

### OP\_CAT operating principe

The working principle of OP\_CAT can be described in just three basic steps:

1. **Data preparation.** Two elements representing the rows of data to be combined are placed on the stack;
2. **Performing the operation.** The concatenation of these strings is then performed with OP\_CAT, creating a new string that contains the combined data of both original strings;
3. **Result to stack.** The concatenation result is placed back on the stack, and the script continues execution based on this new stack state

{% hint style="info" %}
OP\_CAT fails if there are fewer than two values on the stack, or if the combined value is larger than the maximum script element size of 520 bytes (TapScript)
{% endhint %}

An example of using OP\_CAT for beginners:

```
Input Data: "Hello, " "bitcoin world!"

*/ OP_CAT CALL /*

Output Data: "Hello, bitcoin world!"
```

***

### Possibilities of using OP\_CAT in Bitcoin scenarios.

The possibilities of using the OP\_CAT opcode in Bitcoin system scenarios are almost endless, but we can try to highlight the main ones:

* **Smart Contract Construction.** OP\_CAT can be used to create complex scenarios in smart contracts, where string concatenation could be one of the steps to define payment terms or other actions;
* **Integration with external data.** If the blockchain interacts with external data, OP\_CAT can be used to integrate that data with the transaction's internal data;
* **Tree Signatures.** Tree signatures provide a mechanism for creating a multi-signature scenario where the size depends logarithmically on the number of public keys, and can describe conditions of use that go beyond n-of-m. For example, a transaction less than 1 KB in size can support tree signatures with a thousand public keys. This also opens up the possibility of applying generalized logical spending conditions. \[[1](https://github.com/EthanHeilman/op\_cat\_draft/blob/main/cat.mediawiki)]
* **Creating unique transaction labels.** OP\_CAT can be used to create unique transaction labels or identifiers based on the concatenation of various transaction attributes;
* **Creating vaults.** OP\_CAT can be used to create systems in which a user is able to protect their funds from theft if their secret key is compromised by an attacker. \[[2](https://github.com/EthanHeilman/op\_cat\_draft/blob/main/cat.mediawiki)]
* **Combining data for access control.** Within smart contracts, OP\_CAT can be used to create complex access control conditions that depend on a specific combination of data.

***
