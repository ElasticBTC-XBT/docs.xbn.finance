---
description: >-
  Regarding upgradable contracts used by XBN and whether it is safe to hold XBN
  for the long term, please check our explanation below.
---

# TimeLock & Upgradable Proxy Contracts

Transparency is the cornerstone for us and we really really appreciate how so many people have contributed and helped audit our codes so far!

**What is an upgradable contract?**

Upgradable contract making it easy for contract authors to add features and fix bugs in smart contracts. Instead of deploying an actual code, you deploy a pointer to an address where actual code is located. Developers have the ability to change where the pointer points to so that the actual execution will come from a new “upgraded” code.

**What are the pros / cons for upgradable contracts?**

_Pros_: It allows contracts to be changed if bugs or vulnerabilities are found so that the protocol can continue to function safely

_Cons_: Bad actor can maliciously switch contracts and implement new functions / behavior that users did not expect — e.g., steal users’ fund

**So why did XBN use upgradable contracts?**

Without private/pre-sales investors, getting our contracts audited is quite costly for us. We have been testing our codes rigidly we can never be sure if there are bugs, we decided to use upgradable contracts to allow for flexibility.

**How do we know you are not going to rug?**

From 11th October 2021, we will change the owner of all the XBN into the Timelock contract. Hence, any changes made by developers will have a 24 hours lag before becoming effective.

Any questionable changes to the code will provide ample time for users to withdraw funds and exit safely.

In fact, with this set up, if a questionable switch to the implementation contract occurs, you will also have time to react accordingly.



**Timelock contract**: [https://bscscan.com/address/0xB94b6f0c0dFd11a15e437A66d33bc8ECA5A94501#code](https://bscscan.com/address/0xB94b6f0c0dFd11a15e437A66d33bc8ECA5A94501#code)

**XBN contract **: [https://bscscan.com/token/0x547cbe0f0c25085e7015aa6939b28402eb0ccdac#readProxyContract](https://bscscan.com/token/0x547cbe0f0c25085e7015aa6939b28402eb0ccdac#readProxyContract)

**Tx transferring XBN Owner to Time Lock**: [https://bscscan.com/tx/0x946cd931314e9cdedcb2f75ee7b86d6d53ca617888fdec21acf7ff09d2a184b5](https://bscscan.com/tx/0x946cd931314e9cdedcb2f75ee7b86d6d53ca617888fdec21acf7ff09d2a184b5)

**Tx transferring ProxyAdmin Owner to Time Lock**: [https://bscscan.com/tx/0x38fffc8af28a62c9f08a4ddccf42e8d6f9eba261e0bee71c6673ab34957afbef](https://bscscan.com/tx/0x38fffc8af28a62c9f08a4ddccf42e8d6f9eba261e0bee71c6673ab34957afbef)

Finally, once the protocol further develops and we ensure that our contracts do not have any bug or vulnerability, the community will decide whether to continue with this Time Lock mechanism.
