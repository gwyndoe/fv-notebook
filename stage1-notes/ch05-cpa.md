# Chapter 5: Chosen plaintext attacks (CPA)

> Example notes. Rewrite in your own words as you read, and check each point against the book.

## IND-CPA

**Attacker can:** ask the challenger to encrypt any messages it likes, before and after the challenge. Then it submits two messages m0, m1 of equal length and receives the encryption of one of them.

**Attacker wins if:** it guesses which one was encrypted with probability noticeably better than 1/2.

**Why it matters:** it models an attacker who can get the system to encrypt things for them, for example by sending messages and watching the network. A scheme that always gives the same ciphertext for the same message is not secure here, because the attacker can encrypt m0 itself and compare.

**Not covered:** the attacker cannot ask for decryptions. That is CCA (see Chapter 12).

## Open point

Why must m0 and m1 have the same length? Length leaks through ciphertext size, and the definition assumes length is not secret. Confirm against the book.
