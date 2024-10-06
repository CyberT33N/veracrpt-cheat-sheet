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

---

# Summary:
For most users, **AES** offers the best balance of security and performance. **Serpent** and **Twofish** are excellent alternatives if you want stronger security margins, but they come at a performance cost. Cascades like **AES-Twofish-Serpent** provide extreme security but are slower and may be overkill for everyday use.
