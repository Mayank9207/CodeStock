## DESCRIPTION

# Chinese Remainder Theorem

The Chinese Remainder Theorem (CRT) was discovered by the Chinese mathematician Sun Zi.

## Formulation

Let \( m = m₁ × m₂ × ⋯ × mₖ \), where \( mᵢ \) are pairwise coprime. In addition to \( mᵢ \), we are also given a system of congruences:

a ≡ a₁ (mod m₁) a ≡ a₂ (mod m₂) ⋮ a ≡ aₖ (mod mₖ)

where \( aᵢ \) are given constants. The original form of CRT states that the given system of congruences always has **one and exactly one solution modulo \( m \)**.



# Generalized Chinese Remainder Theorem (CRT) for Non-Coprime Moduli

When the moduli m₁, m₂, ..., mₖ are **not pairwise coprime**, the standard Chinese Remainder Theorem cannot be directly applied. However, such systems can still be solved under certain conditions.

---

## Case 1: Moduli Are Not Coprime but the System is Consistent



### General Algorithm for Non-Coprime Moduli

To solve a system of congruences with non-coprime moduli:

1. **Define the System**:
   x ≡ aᵢ (mod mᵢ), for i = 1, 2, ..., k

2. **Check Pairwise Consistency**:
   - For each pair of congruences:
     x ≡ aᵢ (mod mᵢ)
     x ≡ aⱼ (mod mⱼ)

     - Compute gcd(mᵢ, mⱼ) = g.
     - Verify aᵢ ≡ aⱼ (mod g). If this condition is violated, the system is inconsistent.

3. **Combine Consistent Congruences**:
   - Combine congruences iteratively using the least common multiple (lcm) of moduli:
     x ≡ a (mod lcm(mᵢ, mⱼ))

4. **Solve the Final Reduced System**:
   - After reducing all congruences, solve the resulting single congruence.

---

## Example: Solving a System with Non-Coprime Moduli

Solve the system:
x ≡ 2 (mod 6)
x ≡ 3 (mod 9)

### Step 1: Check Consistency
- Compute gcd(6, 9) = 3.
- Verify 2 ≡ 3 (mod 3). This condition is satisfied because both leave a remainder of 2 modulo 3.

### Step 2: Combine Congruences
- Combine the two congruences into one:
  x ≡ 2 (mod lcm(6, 9)) = x ≡ 2 (mod 18)

### Final Solution:
x ≡ 2 (mod 18)

---

## Notes:
- If the system is inconsistent, no solution exists.
- If all moduli are coprime, the standard Chinese Remainder Theorem applies.

## USE OF CHINESE REMAINDER THEOREM IN SOLVING PROBLEMS
