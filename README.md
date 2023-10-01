# Cryptography
Cryptography

Symmetric ciphers - Block Chipers, Stream Ciphers

키스트림이 키에만 의존하는 synchronous stream

암호문에 의존하는 asynchronous stream

대부분 synchronous stream

asynchronous stream 예 -> CFB mode

블록 암호는 한번에 평문 비트들의 전체 블록을 키로 암호화 한다. AES(128ㅠㅑㅅ)

스트림 암호의 보안은 완벽히 키 스트림에 의존, random sequence

RNG(random number generators) -> TRNG need generating session key

-> (General) Pseudorandom Number generator(PRNG)

PRNG는 진정한 의미에서 random이 아님 왜냐면 계산될 수 있고 결정적임

널리 사용되는 것이 ANSI C의 rand() function

CSPRNG

특별한 유형의 PRNG, 예측할 수 없는 PRNG

컴퓨터 과학 or 공학에서 의사난수가 필요한 거의 모든 상황에서 예측 불가능성이 필요하지 X

One-Time-Pad - UnConditional Security - 공격자는 무한한 계산 자원을 가질 수 있기에 무한한 자원으로도 깨지지 않는다면 무조건 정보 이론적으로 안전

모든 key stream은 오직 1번만 사용된다. 키 스트림 비트는 재사용X

```
Kerckhoff's Principle

A cryptosystem should be secure even if the attacker knows all details about the system, with the exception of the secret key.
In particular, the system should be secure when the attacker knows the encryption and decryption algorithms.
```
