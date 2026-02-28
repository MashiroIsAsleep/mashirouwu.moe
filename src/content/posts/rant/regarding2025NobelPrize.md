---
title: Regarding 2025 Nobel Prize in Physics
published: 2026-02-28
description: ''
image: ''
tags: []
category: ''
draft: false 
lang: 'en'
---

There is an obvious question one could ask:

We have already had phenomena such as the Josephson effect and Bose–Einstein condensation described as *macroscopic quantum effects*. So why would **quantum tunneling** deserve this much emphasis again? What exactly distinguishes the older “macroscopic quantum effects” from the one highlighted this time, both conceptually and experimentally?

A compact answer is:

> **“Third quantization” = quantization of the order parameter**  
> that is, **macroscopic energy levels + coherent superposition of macroscopic states**.

## A quantum system formed by single-state condensation

Let us begin with Bose–Einstein condensation. At sufficiently low temperature, the de Broglie wavelengths of many atoms overlap coherently, and a large number of particles occupy the same quantum state. One is then tempted to describe the condensate as a kind of **macroscopic atom**.

Schematically, one may think of the condensate state as

$$
\lvert \mathrm{BEC} \rangle
= \bigotimes_{i=1}^{N} \lvert \psi(x_i)e^{i\phi_i} \rangle .
$$

Each constituent quasi-particle occupies a state with amplitude $\psi(x)$ and phase $\phi$. The essential point is that a huge number of particles are described by one coherent quantum state.

This picture is not limited to atomic gases. In superconductivity, one also encounters a condensed state: the BCS state. In that case the condensation takes place in momentum space rather than ordinary real space, but the spirit is similar: a large number of degrees of freedom become phase coherent.

Now connect two superconductors with a thin insulating barrier. Then one obtains a Josephson junction, where the current is determined by the phase difference between the two superconductors. Formally one may write the Josephson current as

$$
I_J = \langle S(\phi) \rvert [H_T, N_L] \lvert S(\phi) \rangle .
$$

In ordinary metals, electrons suffer resistance because of scattering and interactions. But once electrons form Cooper pairs, they can collectively cross the barrier in a coherent manner.

Still, from Leggett’s viewpoint, this is not yet the deepest sense of a **macroscopic quantum phenomenon**. Why? Because one can still say that this is, in some sense, the accumulated effect of many microscopic quantum objects—many Cooper pairs behaving coherently—rather than the direct quantization of a truly macroscopic collective degree of freedom itself.

The deeper question is therefore:

Can the entire condensate, described by its **order parameter**, behave as a single quantum object with its own quantized levels and even coherent superpositions?

That is the real conceptual leap.

## Quantization of the order parameter: “third quantization”

In 1980, A. J. Leggett argued that previously discussed “macroscopic quantum effects” were not yet enough to prove that quantum mechanics genuinely applies at the macroscopic level in the strongest possible sense.

A large accumulation of microscopic quantum effects is not automatically the same thing as a genuinely macroscopic quantum variable becoming quantized.

So Leggett proposed a sharper target: in a superconducting circuit, one should quantize the **order parameter** itself. If one can show that a macroscopic variable—such as phase, charge, or magnetic flux—has quantized levels and can even exist in a superposition state, then one has much stronger evidence for true macroscopic quantum behavior.

For a superconducting condensate, the macroscopic phase operator $\hat{\phi}$ and number operator $\hat{N}$ satisfy the effective commutation relation

$$
[\hat{\phi}, \hat{N}] = -2i .
$$

This relation suggests that the collective order parameter is not merely a classical field, but may itself be treated quantum mechanically.

To test whether such macroscopic quantization is real, Leggett proposed an idea analogous to Bell’s inequality: the **Leggett–Garg inequality**. The logic is the following.

If a macroscopic observable—say, charge or magnetic flux—has a definite pre-existing value at all times, as a classical picture would assume, then the temporal correlations between measurements taken at different times must satisfy certain classical bounds. But if the system behaves quantum mechanically, these correlations can exceed those classical expectations.

So the problem becomes: find a physical system in which a macroscopically distinguishable degree of freedom can tunnel, quantize, and possibly superpose.

Leggett noticed that a **small Josephson junction** might do exactly this.

## The Josephson junction and the tilted washboard potential

In a current-biased Josephson junction, the order parameter is the phase difference $\phi$ across the junction. Its dynamics can be written in a form analogous to the motion of a particle in an effective potential:

$$
\ddot{\phi}
=
-\gamma \dot{\phi}
-\frac{I_C}{I_0}\sin\phi
+\frac{I}{I_C}.
$$

This produces the famous **tilted washboard potential**. One may picture the phase as a particle trapped in one of the valleys of a washboard that is tilted downhill.

- If the tilt is small enough, the phase remains trapped in a local minimum.
- If the phase escapes, the junction switches behavior.
- The escape can occur either by **thermal activation** over the barrier or by **quantum tunneling** through it.

That distinction is the core of the experiment.

To make the order parameter observable in a more direct way, one typically considers a SQUID geometry, where flux quantization links the superconducting phase to magnetic flux. In that setting, the collective variable is no longer just a formal abstraction: it is tied to a measurable macroscopic quantity.

## The key experiments behind the macroscopic quantum effect

The essential experimental strategy is to compare **classical thermal escape** with **quantum tunneling escape**.

If escape is dominated by thermal activation, then the escape rate should depend strongly on temperature.  
If escape is dominated by quantum tunneling, then it should instead be set by the characteristic plasma frequency and become largely temperature independent at sufficiently low temperature.

That is exactly the crucial signature: as the system is cooled, the measured escape rate eventually stops following the thermal prediction. The curve develops a clear crossover, indicating that thermal activation is no longer the dominant mechanism.

In other words, below a certain temperature, the phase behaves not like a classical object being kicked over the barrier by heat, but like a quantum object tunneling through the barrier.

One natural objection is that such behavior might arise from environmental noise rather than true quantum tunneling. To rule this out, the experiment was repeated using a larger junction, and the same qualitative transition was observed again. This strengthens the claim that the low-temperature saturation is not simply an artifact of noise.

A second experiment probes the existence of **macroscopic quantized levels** more directly. By varying the bias current, one changes the shape of the effective potential $U(\phi)$. If discrete energy levels exist inside the well, then the spacing between them can be tuned, and resonant transitions should appear at specific values of the bias.

Experimentally, such resonant features do appear.

There is some subtlety here: not every resonance peak must be uniquely quantum in origin. Certain nonlinear classical effects, such as Landau-type nonlinear resonance, can in principle mimic part of the signal. However, such explanations account for only part of the observed structure, not the full set of peaks. This is why the quantized-level interpretation remains compelling.

So the significance is not merely “there is tunneling somewhere.” Rather, it is:

1. a **macroscopic collective degree of freedom** is being described quantum mechanically;
2. it exhibits **quantized levels**;
3. it undergoes **tunneling** between states;
4. and in principle, this opens the door to **coherent superpositions of macroscopically distinct states**.

That is the conceptual reason this is qualitatively different from simply saying “many particles are in a quantum state.”

## Why this matters for quantum computation

If one can make the tunneling time long enough and protect coherence well enough, then these macroscopic quantum states can be used as qubits.

This is precisely why superconducting circuits became such an important platform for quantum computation.

A major practical issue in superconducting qubits is noise—especially charge noise. One influential design idea is therefore to use a **small Josephson junction shunted by a large capacitor**, reducing sensitivity to charge fluctuations and improving coherence.

This line of thought directly connects the old foundational question—

> *Can a macroscopic degree of freedom really behave quantum mechanically?*

—to the modern engineering question—

> *Can we stabilize and control that degree of freedom well enough to compute with it?*

Quantum error correction pushes this further by encoding one logical qubit into multiple physical qubits, though this still remains, in many respects, an ongoing technological project rather than a completed practical endpoint.

## Outlook

Can other systems also realize genuinely macroscopic quantum effects?

Quite possibly.

The Gross–Pitaevskii equation for a BEC has a structure reminiscent of the equations governing a small Josephson junction, though with an additional nonlinear term. This suggests that similar ideas about collective variables, tunneling, and coherence may appear in condensate systems as well.

Another important direction is the physics of **anyons** in two dimensions. In two-dimensional systems, particles are not restricted to purely bosonic or fermionic exchange statistics. Instead, one may obtain an additional phase factor upon exchange that is neither $0$ nor $\pi$, but an arbitrary value:

$$
\psi \to e^{i\theta}\psi .
$$

One may heuristically picture this as if the particle carries an attached flux tube, so that braiding two particles generates an extra phase. Such anyonic systems are especially interesting because of their potential use in quantum computation.

## A final question: do white dwarfs and neutron stars count?

Can white dwarfs or neutron stars be called examples of **macroscopic quantum effects**?

A useful distinction is the one between:

- **quantum macroscopicity**: a macroscopic system whose behavior reflects the accumulation of quantum effects;
- **macroscopic quantum behavior**: a macroscopically distinguishable variable that is itself quantized and capable, in principle, of coherent quantum behavior.

Under this distinction, compact stars supported by degeneracy pressure belong more naturally to the **first** category. Their existence certainly depends on quantum mechanics, but that is not quite the same as saying that a macroscopic order parameter has been isolated, quantized, and observed in coherent superposition.

That is the deeper sense in which the Josephson-junction experiments are special.

---

So the real message is this:

The point is not merely that “many microscopic particles behave quantum mechanically.”  
The stronger statement is that a **macroscopic collective variable itself** acquires **discrete quantum levels** and may even participate in **coherent superposition**.

That is the sense in which one may speak of a truly macroscopic quantum phenomenon.