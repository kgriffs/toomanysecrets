# Too Many Secrets (TMS)

TMS is a web service which provides an API for managing encrypted vaults for securely storing and sharing passwords, certificates, keys, etc.

Secrets are encrypted and decrypted by the client; pasphrases are never sent over the wire to the server. This means you don't have to trust your network, or even a remote machine outside your control.

TMS is designed so that even if an attacker posseses the full source code and an understanding of the algorithms involved, he or she will still be unable to decrypt your vaults.

## How it Works (TBD)

Vaults contain safes. Entering the vault passphrase lets you see a list of safes you can open. To open a particular safe, you must have both the vault passphrase and the safe's combination.

Safe's encryption key = AES256(KDF(K+P, Safe's SALT), MKF)

Why?

Group, pin, etc. Splits up - cracking one doesn't give access to others... If an employee leaves, only have to re



## Integrations (TBD)

* SSO (additional layer on top of other passwords)
* UI (web)
* UI (desktop)
* UI (movile)


