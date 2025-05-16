# Grey-Kyber

> [!CAUTION]
> **This should only be used in the game Grey Hack, and is not intended for any real-world applications**
>
This introduces Crystals-Kyber into Grey Hack, a game about hacking.

## Securing SSH passwords in transit
This repository contains an installer script, that will generate a public- and private keypair, and then creates the necessary scripts and config files needed to secure your in-game SSH passwords in transit. 

## Benchmarks
The implementation is considarably fast within the constraints of the game. 
The full encryption and decryption of your SSH password takes less than a second. 
Consider the following rough benchmarks for keygen, encryption and decryption:

|  Method               | time         |
|-----------------------|--------------|
| `Kyber.keygen`        |   ~ 285 ms   |
| `Kyber.encryption`    |   ~ 365 ms   |
| `Kyber.decryption`    |   ~  10 ms   |


## Implement Kyber into something else
Additionally, this repository also contains the plain Kyber implementation, for you to have fun with. 

