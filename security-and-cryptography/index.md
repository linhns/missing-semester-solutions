---
layout: default
title: "Security and Cryptography"
date: 2023-05-09
---

### Question 1
1. Entropy can be calculated by taking log base 2 of possibilities. Since there
   are `100000^4` possibilities, our password will have approximately __66__
   bits of entropy.

2. There are `26` lowercase and uppercase letters, together with `10` digits,
   which give us a total of `62` alphanumeric characters. With our password
   being 8 characters long, that leaves us with `36^8` possible options. Thus
   entropy is __48__ bits.

3. First password is stronger as it has higher entropy.

4. In a year, the attacker can guess `365 * 24 * 60 * 60 * 10000 = 315360000000` 
times.
  * First password: `100000 ^ 4 / 315360000000 = 3.17 * 10^8` years.
  * Second password: `62 ^ 8 / 315360000000 = 692` years.
