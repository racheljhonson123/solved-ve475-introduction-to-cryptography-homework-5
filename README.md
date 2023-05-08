Download Link: https://assignmentchef.com/product/solved-ve475-introduction-to-cryptography-homework-5
<br>
<strong>Ex. 1 –</strong><em> RSA setup</em>

Most RSA setups require the message m to be coprime to the RSA modulus n. In the exercise we will prove that m can still be decrypted if gcd(m, n) is not 1.

<ol>

 <li>Why is it likely for n to be coprime with m ?</li>

 <li>Let k be a multiple of (n).</li>

 <li>Show that if gcd(m, n) = 1 , then m<sup>k</sup> ≡ 1 mod p and mod q.</li>

 <li>Prove that for any arbitrary m, m<sup>k+1</sup> m mod p and mod q.</li>

 <li>Let e and d the RSA encryption and decryption exponent, respectively.</li>

 <li>Show that m<sup>ed</sup> ≡ m mod n for all m.</li>

 <li>Conclude on the necessity of having gcd(m, n) = 1.</li>

</ol>

<strong>Ex. 2 –</strong><em> RSA decryption</em>

The ciphertext 5859 was obtained using RSA encryption with n = 11413 and e = 7467. Recover the plaintext.

<strong>Ex. 3 –</strong><em> Breaking RSA</em>

Wiener’s attack allows to recover the decryption exponent under the condition that it is small enough.

<ol>

 <li>Why would one select short encryption or decryption keys?</li>

 <li>Search and explain how Wiener’s attack is working.</li>

 <li>How to ensure not generate a weak decryption key?</li>

 <li>Given n = 317940011 and e = 77537081, apply Wiener’s attack in order to factor n. Either provide the source code of your program or clearly detail all the steps.</li>

</ol>

<strong>Ex. 4 –</strong><em> Programming</em>

Implement the three functions generate, encrypt and decrypt, which generate the RSA parameters, encrypt, and decrypt, respectively.

The function generate takes as input a security level and generate p and q such that n is long enough to match the required security level. No special requirement is requested on encrypt and decrypt.

Common security levels:




<table>

 <tbody>

  <tr>

   <td width="141">Security level (bits)</td>

   <td width="46">80</td>

   <td width="46">112</td>

   <td width="46">128</td>

   <td width="47">192</td>

   <td width="54">256</td>

  </tr>

  <tr>

   <td width="141">RSA modulus (bits)</td>

   <td width="46">1024</td>

   <td width="46">2048</td>

   <td width="46">3072</td>

   <td width="47">7680</td>

   <td width="54">15360</td>

  </tr>

 </tbody>

</table>




<strong>Ex. 5 –</strong><em> Simple questions</em>

Let n, e, d, p, q be the usual RSA parameters.

<ol>

 <li>A message m is encrypted into the ciphertext c. Explain how to run a CCA attack on “texbook RSA”.</li>

 <li>Instead of using a single exponent one wants to encrypt twice using a single n but two different exponents. Is this double encryption adding any security ?Explain your answer.</li>

 <li>Let n = 642401. Knowing that 516107<sup>2</sup> ≡ 7 mod n and 187722<sup>2</sup> ≡ 4 7 mod n factorize n.</li>

 <li>Describe how an RSA scheme would work if instead of the two primes p and q, three primes p, q, and r were used. Explain the drawback of such a setup.</li>

 <li>Determine the smallest generator of U(Z/97Z).</li>

 <li>Consider the multiplicative group G = U(Z/101Z).</li>

 <li>Prove that 2 is a generator of G.</li>

 <li>In G, determine log2 24, knowing that log2 3 = 69.</li>

 <li>In G, determine log2 24, knowing that log2 5 = 24.</li>

 <li>Knowing that<sup> 3</sup><sup>6</sup> ≡44 mod 137, and<sup> 3</sup><sup>10</sup> ≡2 mod 137, find 0 ≤ x ≤ 135 such that 3<strong>X </strong>≡ 11 mod 137.</li>

 <li>Let G = U(Z/11Z)</li>

 <li>Compute 6<sup>5</sup> in G.</li>

 <li>Prove that 2 is a generator of G</li>

 <li>Let x be such that 2′ ≡ 6 mod 11. Without calculating it, decide whether x is even or odd.</li>

</ol>

<strong>Ex. 6 –</strong><em> DLP</em>

In this exercise we want to determine x such that<sup> 3</sup><strong><sup>X</sup></strong> ≡2 mod 65537.

<ol>

 <li>Prove that 2048 divides x, while 4096 does not.</li>

 <li>How many possible choices need to be considered for x ?Determine x.</li>

 <li>Can the Pohlig-Hellman algorithm be applied to this example ? If so show the details.</li>

 <li>Explain why such primes are not fitting a cryptographic context.</li>

</ol>

<em>Note:</em> in homework 4 exercise 2 it was proved that 3 is a generator of U(Z/65537Z).