# veracrpt-cheat-sheet




# VeraCrypt Encryption Algorithms Ranking

## 1. **AES (Advanced Encryption Standard)**
- **Strength**: AES is the most widely used encryption standard and is trusted by governments, corporations, and security professionals worldwide. It’s known for its balance between speed and security.
- **Performance**: AES is highly optimized for modern CPUs, offering the best performance with hardware acceleration (AES-NI).
- **Use Case**: Recommended for most users because it’s secure and efficient.

## 2. **Serpent**
- **Strength**: Serpent is considered one of the most secure block ciphers due to its conservative design. It was one of the final candidates in the AES competition and is known for resisting cryptographic attacks.
- **Performance**: Slower than AES but offers a higher security margin.
- **Use Case**: Ideal for those who prioritize security over speed.

## 3. **Twofish**
- **Strength**: Twofish was another AES finalist. It’s highly secure and features a balanced design between speed and security. It’s also unpatented and freely available.
- **Performance**: Slower than AES but faster than Serpent in most implementations.
- **Use Case**: A great alternative to AES, especially for those who prefer a non-patented algorithm.

## 4. **Camellia**
- **Strength**: Camellia offers security comparable to AES and is widely used in Japan and Europe. It has undergone extensive scrutiny and is certified by NESSIE and ISO/IEC.
- **Performance**: Similar performance to AES, especially on 64-bit platforms.
- **Use Case**: Another strong choice, but less popular than AES.

## 5. **Kuznyechik (GOST R 34.12-2015)**
- **Strength**: Kuznyechik is a Russian encryption standard. It has a robust design, but it hasn't been scrutinized as thoroughly in the West as other algorithms like AES or Serpent.
- **Performance**: Reasonably efficient but less tested in global cryptographic communities.
- **Use Case**: Suitable for those looking for a non-Western encryption standard.

---

# Cascading Algorithms

## 6. **AES-Twofish-Serpent**
- **Strength**: Cascading three strong algorithms increases security, assuming none of the ciphers have been broken. Even if one cipher is compromised, the others remain secure.
- **Performance**: Significantly slower due to the triple encryption process.
- **Use Case**: Extreme security with performance trade-offs. Ideal for highly sensitive data.

## 7. **Serpent-Twofish-AES**
- **Strength**: Similar to the above cascade but orders the ciphers differently. Serpent, being the slowest, comes first, making this combination slightly less efficient.
- **Performance**: Slower than AES-Twofish-Serpent.
- **Use Case**: Extremely secure, but the performance hit makes it less practical for regular use.

## 8. **Twofish-Serpent**
- **Strength**: A dual-cascade offering robust encryption by combining Twofish and Serpent.
- **Performance**: Better performance than triple cascades, but slower than single-algorithm encryption.
- **Use Case**: A good compromise between speed and multi-layered security.







<br><br>
<br><br>



# VeraCrypt Hash Algorithms Ranking

## 1. **SHA-512 (Secure Hash Algorithm 512-bit)**
- **Strength**: SHA-512 offers a very high level of security with a 512-bit output, making it highly resistant to collisions and brute-force attacks. It’s widely used and trusted across many applications.
- **Performance**: Though slower than SHA-256 due to its larger bit size, SHA-512 is still efficient on modern hardware.
- **Use Case**: Ideal for users who want maximum security without significant performance compromises.

## 2. **Whirlpool**
- **Strength**: Whirlpool produces a 512-bit hash and is designed specifically for cryptographic security. It hasn’t seen widespread use like SHA-512 but is still regarded as very secure and resistant to all known attacks.
- **Performance**: Slower than SHA-512, especially on older hardware.
- **Use Case**: Great for users who prefer non-SHA alternatives with high security margins, but the performance can be a downside.

## 3. **SHA-256 (Secure Hash Algorithm 256-bit)**
- **Strength**: SHA-256 is one of the most popular hash algorithms and is used in many security protocols, including SSL, TLS, and Bitcoin. It’s highly secure with a 256-bit output and has withstood years of cryptanalysis.
- **Performance**: Faster than SHA-512, making it a good balance between security and speed.
- **Use Case**: The go-to choice for most users who want a highly secure but faster hashing algorithm than SHA-512.

## 4. **Streebog (GOST R 34.11-2012)**
- **Strength**: Streebog is a Russian hashing standard, available in 256-bit and 512-bit versions. While secure, it has seen less scrutiny in Western cryptographic communities.
- **Performance**: Reasonably efficient, but not as optimized or as fast as SHA-256.
- **Use Case**: Suitable for those looking for a non-Western hash standard with good security, though less tested globally.

---

# Summary:
For most users, **SHA-512** offers the best combination of security and performance. **Whirlpool** is also a solid option but may be slower, and **SHA-256** strikes a perfect balance between speed and security. **Streebog** is an interesting choice for those seeking alternatives to SHA, but it’s less widely trusted.


---

# Summary:
For most users, **AES** offers the best balance of security and performance. **Serpent** and **Twofish** are excellent alternatives if you want stronger security margins, but they come at a performance cost. Cascades like **AES-Twofish-Serpent** provide extreme security but are slower and may be overkill for everyday use.
