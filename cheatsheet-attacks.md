# Cheat sheet: attack powers

> Example. Rewrite from what you have read.

| Attacker | Can do | Protects against | Breaks which scheme |
| --- | --- | --- | --- |
| Eavesdropper | Sees ciphertexts only | Passive network sniffing | Schemes with obvious patterns |
| Chosen plaintext (CPA) | Also gets encryptions of its own messages | Attacker influences what gets encrypted | Deterministic encryption |
| Chosen ciphertext (CCA) | Also gets decryptions of its own ciphertexts | Attacker tampers with ciphertexts and sees the results | Schemes that can be modified without detection (malleable) |
