Practice using Zokrates
Use Remix
Install the Zokrates plugin

1. Use the example file to generate a proof to show that a
prover knows the square root of 25.

Answer: proof.json
{
  "scheme": "g16",
  "curve": "bn128",
  "proof": {
    "a": [
      "0x133fe11a18ca93be2111c5261519cb28a20f2d43878aad077ddd8f98ec1698a8",
      "0x1189caa6dd07d9f49547231b6f9da412aa521209c651e7375c52c06bac4450b7"
    ],
    "b": [
      [
        "0x1770b446c79b32d25c8d64dad1f5f107d801ff1373956363f53c379666966729",
        "0x1aa92fa3946d2c18c3f20be33d5af3f4a6465d65d4c2ba9e8a984939acef96cc"
      ],
      [
        "0x2ce5f64ef6ea33e888aa2eb6a5c7abce2f398cd4cd6a0ebf66299520f7c8d7dd",
        "0x08bbd31c833e8c841d1ff18072eba3c99434db58d14bee690557bc4c44919304"
      ]
    ],
    "c": [
      "0x2913de8093dc2870515d1a64ceaffcd5278f67253388257604f0d82bf3d79eb1",
      "0x18babbac2aec8a75a375ca2e6aae43d8bd19c62840a032af5ebd70684243a01f"
    ]
  },
  "inputs": [
    "0x0000000000000000000000000000000000000000000000000000000000000019"
  ]
}

2. Try to create an invalid proof

Answers:
Zokrates limits the options of what can you provide as witness for a compiled program. 
For a = 4, b = 25, you get 'Execution failed: Assertion failed at main.zok:2:5'
For a = 5, b = -1 (or some string) you get 'Type error: Could not parse `-1` to field type'. It seems like the values are limited to Z (whole numbers)
For a = -1, b = 1, it still doesn't work, so seems like negative numbers are not the options.

*Field element is [0, p - 1], where p is a large prime number.*


3. Follow the example to build a proof that you know the pre image of a hash https://zokrates.github.io/examples/sha256example.html 

Answers:
(48886 constraints) 


4. In principle how could you use Zokrates to verify that a certain address on Ethereum has more than say 1 ETH ?

Answers:
Perhaps we can take in private field address, using some lib read the balance and assert that it is bigger than 1 ETH.


