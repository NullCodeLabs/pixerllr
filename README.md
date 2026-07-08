# pixerllr

> **Reality fingerprints for AI video — extracting motion, light, wind, water, space, and anatomy priors from real footage, without storing the footage.**

A six-fingered hand is not an artistic choice.
A floating body is not a style.
A shadow falling the wrong way is not atmosphere.

**It is an error — and you pay for it with every burned credit and every discarded generation.**

AI video generators do not understand physics.
Not because they are stupid — because nobody has ever taught them.

Their training data is full of studio lighting, wind machines, wires, and mixing desks.
The model learns what it sees: **cinematic physics**.

And cinematic physics lies.

**pixerllr addresses the root cause — it does not patch the symptoms.**

---

## What it does

From real footage — live-action film, nature footage, candid video — pixerllr extracts the laws of reality:

* **Anatomy and gravity**
  How a real body moves.

* **Aging**
  How gait stiffens and skin wrinkles across decades.

* **Natural light**
  Where a shadow falls when the Sun is the light source.

* **Wind**
  How reeds, leaves, and hair bend.

* **Water**
  How a wave propagates when nobody staged it.

* **Space**
  Depth in the image, resonance in the sound — whether the world is open or closed.

The extracted law is stored as a fingerprint:

```text
skeleton sequence
response curve
spatial fingerprint
```

One JSON record per video.

**The image is discarded. The law remains.**

This becomes a reference library from which generative models can learn what they currently do not know:

**how to make lifelike film.**

Not plausible.
**Lifelike.**

---

## The machine

```text
SOURCE      → archive branch: film, nature footage
             + crowd branch: personal camera footage

EXTRACTION  → lightweight layer on CPU
             + heavy layer on free GPU

FINGERPRINT → JSON record, hash-keyed, image-free

LIBRARY     → law curves:
               wind ↔ foliage
               sun ↔ shadow
               age ↔ gait

PACKAGE     → prior modules
             + loss library
             + pointer dataset

VALIDATION  → measurably fewer physical errors,
               or it is worth nothing
```

Every component is built on open tools.

We did not invent what already works — we connected what nobody had connected before.

---

## Two modes — the reality gate

### 1. Measuring instrument

You can score any video, including AI-generated video.

You learn where it lies about physics:

* hands
* shadows
* wind
* floating bodies
* motion
* space
* consistency

In numbers.

Your discarded generation becomes a lesson.

**You get a report. Nothing is stored.**

---

### 2. Teacher

Only real footage may enter the library.

A three-layer gate protects it:

1. **Origin verification**
2. **Metadata coherence**
3. **Physical correlation**

Real footage correlates with measured wind and computed solar position.

Generated footage does not.

What fails the gate does not enter.

> **Your discarded generation is a lesson.
> Your reference footage is treasure.**

---

## What you get — and what the commons gets

Run the instrument and you get an immediate report.

**Free. No strings attached.**

If the fingerprint of your real footage passes the gate, you become a contributor.

As a contributor, you get:

* full-resolution access to all curves in the reference library;
* named, citable acknowledgment;
* early access to prior packages;
* pretrained physics-knowledge modules that can be connected to your own workflow;
* fewer failed generations;
* fewer burned credits.

The license is our contract.

The data and the library are released under:

```text
CC BY-NC-SA 4.0
```

Free for everyone for non-commercial use.

Anyone who wants to build it into a product needs a commercial license.

**You build it, you use it for free.
Whoever makes money from it helps sustain it.**

This is the OpenStreetMap model, and it has worked for twenty years.

---

## What we do not do

* **We do not store or distribute video. Ever.**
  The record is metadata and a pointer — the same model used by the largest open datasets.

* **We do not preserve faces, identities, or scenes.**
  The fingerprint contains no image and no biometric data — only what is true across domains.

* **We do not train on AI-generated material.**
  We measure it — but we learn from reality.

* **We do not learn music, dubbing, or mixed soundtrack content.**
  The spatial fingerprint of location sound — resonance, open or closed space — is a law, and it enters.

---

## Getting started — zero installation

1. Open the fingerprint form:

   ```text
   Issues → New
   ```

2. Paste a video URL.

3. Submit it.

4. Our machine does the work.

5. You receive a link to your report.

6. The fingerprint enters the library automatically if it passes the reality gate.

Already returning, and want to run it on your own machine?

**Fork the repo — the user guide explains the rest.**

---

## Related pattern

This README follows the narrative-technical GitHub format used in [`Human2ai-intent-codec`](https://github.com/NullCodeLabs/Human2ai-intent-codec):

* strong opening claim;
* human problem;
* technical answer;
* clear operating model;
* contributor value;
* explicit ethical boundaries;
* immediate path to start.

---

## Status

```text
v0.1 — under construction
```

Done:

* schema;
* repo skeleton;
* source hierarchy.

Next:

* extraction scripts;
* validator workflow;
* first law curves.

---

## Contributing

If you see what we see:

**Star.**

If you would use it:

**Fork.**

If you find a bug or know a better path:

**Open an Issue — that is what we read first.**

---

## License

© Infinity Possibility Media Co. | NullCodeLabs

Data and documentation:

```text
CC BY-NC-SA 4.0
```

Commercial use requires a separate license.

---

## Contact

* Email: `istvan.taubert@gmail.com`
* GitHub: [`@NullCodeLabs`](https://github.com/NullCodeLabs)
