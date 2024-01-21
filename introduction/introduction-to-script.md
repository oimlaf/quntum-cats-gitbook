---
description: Basic definitions of the Script language
---

# 📘 Introduction to Script

In the world of Bitcoin, a special and unique scripting language called "Script" is used. This language is a perfectly crafted programming dialect. The Bitcoin scripting language is based on a stack architecture, where all data is stored on a stack, and operations are performed on that stack.

Bitcoin Script is not a Turing-complete language. A Turing-complete language has properties that allow it to solve any computational problem, but Script has limitations that make it not Turing-complete. The following are the main reasons why this is the case:

* **Limited stack size**. Script uses the stack to process data and commands. However, Bitcoin has limited stack size to prevent abuse and unlimited resource consumption;
* **Lack of loops.** Turing-complete languages typically support loops to allow repetitive operations. Script does not provide full-fledged loop constructs, which limits programming options;
* **Lack of branching operators**. Script supports conditional statements, but does not have full branching operators such as "if-else", which makes it impossible to create complex branching program structures;
* **Limited arithmetic capabilities**. Operations in Script are limited to basic arithmetic operations, and there is no support for complex mathematical calculations;
* **Lack of I/O support**. Script has no mechanisms for interacting with external data sources or I/O devices.

All these restrictions in Script were put in place to ensure security and prevent possible attacks on the Bitcoin network.
