# Semantic security versus IND-CPA

> Example. Rewrite from what you have read in Chapters 2 and 5.

**Semantic security** says the ciphertext tells the attacker nothing useful about the plaintext.

**IND-CPA** says the attacker, who can encrypt messages of its choice, cannot tell which of two messages was encrypted.

They are two ways to state the same goal for encryption. Semantic security is the intuition. IND-CPA is the form that is easy to prove things about and to extend: adding decryption access gives IND-CCA.

## What I'm unsure about

Whether the book's "semantic security" game is already the two-message form. Check Chapters 2 and 5.
