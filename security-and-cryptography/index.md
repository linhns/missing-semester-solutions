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

### Question 2
Instructions here are for Linux and Debian version `11.7.0` accordingly. Substitute
suitable values depending on your OS.
```bash
curl -LO
http://debian.xfree.com.ar/debian-cd/current/amd64/iso-cd/debian-11.7.0-amd64-netinst.iso
sha256sum debian-11.7.0-amd64-netinst.iso
```
Since the hash computed with `sha256sum` for the file downloaded from
Argentinian mirror matches what listed on Debian website, this mirror is legit.
