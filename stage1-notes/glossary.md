# Glossary

> Example entries. Add one line per term as you meet it, in your own words.

- **Adversary / attacker:** the algorithm trying to break the scheme.
- **Challenger:** the algorithm that runs the game and plays the honest side.
- **Game:** a fixed script of moves between challenger and adversary, ending in a win or a loss.
- **Oracle:** a service the attacker may call, for example "encrypt this for me".
- **Advantage:** how much better than guessing the attacker does, for example |Pr[win] - 1/2| in the bit-guessing form.
- **IND-CPA:** attacker can encrypt chosen messages, and must tell which of two chosen messages was encrypted.
- **IND-CCA:** IND-CPA, plus the attacker can ask for decryptions of ciphertexts of its choice (except the challenge itself).
- **Negligible:** smaller than any inverse polynomial in the key size.
