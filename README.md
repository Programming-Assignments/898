Download Link: https://assignmentchef.com/product/898
<br>
<h2>1.1           Part 1: Analyzing the generator</h2>

<ol>

 <li>a) We’ve been given the generator <em>g </em>= 18 and we are working in Z<sub>23</sub><sup>∗</sup>. The group which it generates is the set <em>&lt; g &gt;</em>= <em>S </em>= {<em>g<sup>i</sup></em>|0 ≤ <em>i </em>≤ 21}.</li>

</ol>

A table for the calculations that find this set:

<table width="558">

 <tbody>

  <tr>

   <td width="35">i</td>

   <td width="23">0</td>

   <td width="30">1</td>

   <td width="23">2</td>

   <td width="30">3</td>

   <td width="23">4</td>

   <td width="23">5</td>

   <td width="23">6</td>

   <td width="23">7</td>

   <td width="30">8</td>

   <td width="30">9</td>

   <td width="30">10</td>

   <td width="30">11</td>

   <td width="30">12</td>

   <td width="30">13</td>

   <td width="30">14</td>

   <td width="30">15</td>

   <td width="30">16</td>

   <td width="30">17</td>

   <td width="28">…</td>

  </tr>

  <tr>

   <td width="35">g^i</td>

   <td width="23">1</td>

   <td width="30">18</td>

   <td width="23">2</td>

   <td width="30">13</td>

   <td width="23">4</td>

   <td width="23">3</td>

   <td width="23">8</td>

   <td width="23">6</td>

   <td width="30">16</td>

   <td width="30">12</td>

   <td width="30">1</td>

   <td width="30">18</td>

   <td width="30">2</td>

   <td width="30">13</td>

   <td width="30">4</td>

   <td width="30">3</td>

   <td width="30">8</td>

   <td width="30">6</td>

   <td width="28">…</td>

  </tr>

 </tbody>

</table>

where the ’…’ represent that the calculations continue, however in the same cyclical pattern as previously. The set <em>S </em>= {1<em>,</em>2<em>,</em>3<em>,</em>4<em>,</em>6<em>,</em>8<em>,</em>9<em>,</em>12<em>,</em>13<em>,</em>16<em>,</em>18}.

<ol>

 <li>b) We note 2 · 3 = 6 ∈ <em>S</em>,</li>

</ol>

2 · 4 = 8 ∈ <em>S</em>,

4 · 6 (mod 23) = 1 ∈ <em>S,</em>

3 · 4 = 12<em>,</em>∈ <em>S</em>

3 ·16 (mod 23) = 2 ∈ <em>S.</em>

Proposition 1. <em>Let </em><em>q &gt; </em>0 <em>and </em><em>g </em>∈ Z<sub>p</sub><sup>∗ </sup><em>and has the property </em><em>g<sup>q </sup></em>= 1 <em>then </em>{<em>g<sup>i</sup></em>|0 ≤ <em>i &lt; q</em>} <em>is closed under scalar multiplication.</em>

Proof We want to show that for given any <em>a,b </em>∈ <em>S </em>= {<em>g<sup>i</sup></em>|0 ≤ <em>i &lt; q</em>} then <em>a </em>· <em>b </em>∈ <em>S</em>.

Let <em>a </em>= <em>g<sup>k</sup></em><sup>1 </sup>and <em>b </em>= <em>g<sup>k</sup></em><sup>2</sup>, then <em>a</em>·<em>b </em>= <em>g<sup>k</sup></em><sup>1</sup><sup>+<em>k</em></sup><sup>2</sup>. Let us distinguish between two cases that can happen. Case 1: <em>k</em><sub>1</sub>+ <em>k</em><sub>2 </sub><em>&lt; q</em>, then the result is clear that <em>a </em>· <em>b </em>∈ <em>S </em>by definition of <em>S</em>.

Case 2: <em>k</em><sub>1</sub>+<em>k</em><sub>2 </sub>≥ <em>q</em>. Note that <em>k</em><sub>1</sub>+<em>k</em><sub>2 </sub><em>&lt; </em>2<em>q </em>from defintion of S and hence we can write <em>k</em><sub>1</sub>+<em>k</em><sub>2 </sub>= <em>q</em>+<em>s </em>where we know 0 ≤ <em>s &lt; q</em>. <em>g<sup>k</sup></em><sup>1</sup><sup>+<em>k</em></sup><sup>2 </sup>= <em>g<sup>q</sup></em><sup>+<em>s </em></sup>= <em>g<sup>q </sup></em>· <em>g<sup>s </sup></em>= 1 · <em>g<sup>s </sup></em>= <em>g<sup>s </sup></em>∈ <em>S</em>.

In both cases we conclude that <em>a </em>· <em>b </em>∈ <em>S </em>and this concludes the proof.

<h2>1.2           Part 2: Encrypting a message</h2>

We know that the public key is 6 = <em>g<sup>x </sup></em>and the message <em>m </em>= 17. By looking at our table from previous part we note that <em>x </em>= 7. To encrypt <em>m </em>we choose a random , in this case we choose <em>k </em>= 3. We encrypt by calculating <em>c </em>= (<em>c</em><sub>1</sub><em>,c</em><sub>2</sub>).

Calculate . Hence <em>c </em>= (13<em>,</em>15)<em>.</em>

To assure ourselves that we have encrypted the correct way we can try to decrypt the message in this case. We can do this since we know the fact that <em>x </em>= 7. We start with calculating <em>k </em>= 13<sup>7 </sup>= 9 in , where <em>k</em><sup>−1 </sup>can be found using the extended euclidean algorithm and in this case we get since , that . Performing this calculation gives us then that  and we obtain the original message.

<h2>1.3           Part 3: Decrypting a message</h2>

What is public is that we are using the group G = (the order of the generated set), and also <em>h </em>= <em>g<sup>x </sup></em>= 18<sup>9 </sup>= 12 (mod 23). So we can write public key pk = (<em>G,g,q,h</em>)

We have the message (13,11)(12,15)(9,10) and the private key <em>x </em>= 9. Since we have the private key we can follow the steps to decipher this message.

We use the formula that and . These calculations in our case when <em>p </em>= 23 and we essentially have three different messages we wish to decrypt and then concatenate these into the secret message.

<em>k </em>= 13<sup>9 </sup>= 3 (mod 23), <em>k</em><sup>−1 </sup>= 8 since 3 · 8 = 1 (mod 23). We then get <em>m </em>= 11 ∗ 8 = 19 (mod 23). This letter is ’S’.

<em>k </em>= 12<sup>9 </sup>= 4 (mod 23), <em>k</em><sup>−1 </sup>= 6 since 4 · 6 = 1 (mod 23). We then get <em>m </em>= 15 ∗ 6 = 21 (mod 23). This letter is ’U’.

<em>k </em>= 9<sup>9 </sup>= 2 (mod 23), <em>k</em><sup>−1 </sup>= 12 since 2 · 12 = 1 (mod 23).We then get <em>m </em>= 10 ∗ 12 = 5 (mod 23). This letter is ’E’.

The concatenated decrypted word is then: ’SUE’.

In this example finding the inverses were quite straightforward and the solution were ’seen’. In the general way one would use the extended euclidean algorithm to find <em>k</em><sup>−1</sup>. This is how these calculations would look for the first case, i.e the letter ’S’ using the extended euclidean algorithm.

3

<em>k </em>= 3, and we wish to find <em>k</em><sup>−1 </sup>in (mod 23).

23 = 3 · 7+2

3 = 2 · 1+1

2 = 1 · 2+0

Then we move backwards

1 = 3 − 2 · 1

1 = 3 − (23 − 3 · 7) = 3 · 8 − 23

Which gives us that if we take (mod 23) on both sides, we obtain that 3 · 8 = 1 (mod 23)

Written in python-like code (where % is modulus and // is integer division) we can write the EEA algorithm recursively as follows

Algorithm 1 EEA(a, b)

1: if a == 0 then

2:             return (<em>b,</em>0<em>,</em>1)

3: else

4:                 gcd, x, y = EEA(b % a, a)

5:                return (gcd, y – (b//a) * x, x)

I believe the steps in calculation is easier to show by example as we did above but the algorithm can also be used.

4