

## From Diffusive to Ballistic Transport

**Reading source:** Supriyo Datta, *Lessons from Nanoelectronics: B. Quantum Transport*, Chapter 1, Sections 1.1–1.3 (Conductance, Ballistic Conductance, and What Determines the Resistance?).

## 1. Why does the transport picture change at the nanoscale?

In a diffusive conductor, electrons undergo scattering as they move through the channel. Their motion can be viewed, at a basic level, as a sequence of segments interrupted by scattering events. The mean free path, usually written as `lambda` (λ), is the average distance an electron travels before a relevant scattering event.

When the channel length `L` is much longer than the mean free path, transport is typically diffusive. When `L` is much shorter than the mean free path, electrons can cross the channel with little scattering inside it; this is the ballistic regime.

- **Diffusive regime:** `L >> λ`
- **Ballistic regime:** `L << λ`
- **Intermediate regime:** `L` is comparable to `λ`

These are limiting regimes of a continuous transport picture, not two completely separate types of physics.

## 2. Classical conductance

For a uniform conductor in the ohmic regime,

$$
R = \frac{V}{I} = \rho\frac{L}{A}
$$

and therefore

$$
G = \frac{I}{V} = \sigma\frac{A}{L},
$$

where:

- `R` is resistance,
- `G` is conductance,
- `ρ` is resistivity,
- `σ = 1/ρ` is conductivity,
- `L` is the channel length, and
- `A` is its cross-sectional area.

This description is useful for diffusive conductors. At the nanoscale, however, the number of available quantum transport modes and the contacts can become important parts of the conductance picture.

## 3. Ballistic conductance

For an ideal ballistic conductor, Datta writes the conductance as

$$
G_B = \frac{q^2}{h}M,
$$

where:

- `G_B` is the ballistic conductance,
- `q` is the magnitude of the electron charge,
- `h` is Planck's constant, and
- `M` is the number of effective conducting modes (transport channels).

The factor `q²/h` is approximately `38.7 μS`, often rounded to `40 μS`. Thus, in this mode-counting convention, each effective mode contributes one conductance unit of `q²/h`.

**Important:** The value of `M` depends on how the conducting modes and degeneracies (for example, spin) are counted. The expression above follows the convention used in Datta's text.

## 4. What connects the two regimes?

The book gives a useful interpolation for the conductance of a conductor with channel length `L` and mean free path `λ`:

$$
G = \frac{G_B}{1 + L/\lambda}.
$$

It has the expected limits:

- If `L << λ`, then `G` approaches `G_B` (ballistic limit).
- If `L >> λ`, then `G` is approximately `G_B λ/L` (diffusive limit).

This makes an important point: ballistic and diffusive transport are connected through the ratio of channel length to mean free path.

## 5. Why does this matter for nanoscale magnetic devices?

In nanoscale magnetic devices, the transport length can be comparable to microscopic scattering lengths, so a purely classical, bulk-resistivity picture may not be sufficient. A quantum-transport description allows us to discuss conducting modes, contacts, and transmission probabilities.

For magnetic tunnel junctions, spin-dependent transmission and tunneling through the barrier must also be considered. The ideal ballistic expression above is a useful conceptual reference, but it is **not by itself a complete conductance formula for a magnetic tunnel junction**.

## 6. Key takeaways

1. The ratio `L/λ` helps identify whether transport is mainly diffusive, ballistic, or intermediate.
2. In the ballistic limit, conductance is related to the number of available transport modes.
3. A ballistic conductor does not automatically have zero resistance; contacts and the available modes matter.
4. Quantum transport provides a framework for moving beyond a simple bulk-resistivity description at the nanoscale.

## 7. Questions for further study

- What determines the number of available modes `M` in a given material and geometry?
- How does a scattering region reduce the transmission of each mode?
- How is the ballistic conductance picture generalized when transmission is less than one?
- How do spin polarization and a tunnel barrier modify transport in a magnetic tunnel junction?

## References

- Datta, S., *Lessons from Nanoelectronics: B. Quantum Transport*, Chapter 1, especially Sections 1.1–1.3, World Scientific, 2nd edition (2017).
- [Available course text (PDF)](https://courses.edx.org/asset-v1:PurdueX+69503x+3T2018+type@asset+block@Datta-LNE-Part-B-2nd-WorldScientific.pdf)

---

*This note is an original study summary written in my own words. It is not a reproduction of the textbook.*
