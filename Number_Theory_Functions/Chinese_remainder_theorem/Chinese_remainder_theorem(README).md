## DESCRIPTION

# Chinese Remainder Theorem

The Chinese Remainder Theorem (CRT) was discovered by the Chinese mathematician Sun Zi.

## Formulation

Let \( m = m₁ × m₂ × ⋯ × mₖ \), where \( mᵢ \) are pairwise coprime. In addition to \( mᵢ \), we are also given a system of congruences:

a ≡ a₁ (mod m₁) a ≡ a₂ (mod m₂) ⋮ a ≡ aₖ (mod mₖ)

where \( aᵢ \) are given constants. The original form of CRT states that the given system of congruences always has **one and exactly one solution modulo \( m \)**.



### Condition for Solving the System of Congruences

For the system of congruences:
x ≡ a₁ (mod m₁) x ≡ a₂ (mod m₂)

The solution exists if and only if the following condition holds:

gcd(m₁, m₂) | (a₂ - a₁)

Where:
- `gcd(m₁, m₂)` is the greatest common divisor (GCD) of the moduli `m₁` and `m₂`,
- `a₁` and `a₂` are the respective remainders.

This condition means that the difference between `a₂` and `a₁` must be divisible by the greatest common divisor of `m₁` and `m₂` for the system to have a solution.

