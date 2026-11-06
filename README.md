<div align="center">

# KalpaXi

**Design it. Check it. Make it.**

Open-source CAD with engineering checks built in — from idea to proven part, on one model.

</div>

---

## What is KalpaXi?

KalpaXi is a parametric CAD program for mechanical design where **the engineering checks live inside the model**.
You design a part, put parts together, make the manufacturing drawing, and then check the design —
stress, heat, fatigue, tolerances and manufacturability — without exporting, re-meshing by hand or switching programs.

**Change a size and everything that uses it follows:** the assembly, the drawing, the mesh and the analysis results.

*Kalpa* (कल्प) — idea, design, the proper way of doing a thing.
*X* — examine every design.
*i* — intelligence, the assistant that helps along the way.

## Why

Good ideas slow down between the CAD tool, the analysis tool and the drawing board.
Each handover means exporting files, rebuilding geometry and checking whether everything still matches.
KalpaXi keeps one model as the single source of truth, so engineers, makers and small teams can go from concept to a checked, manufacturable part fast.

## Capabilities

| Area | What it does | Status |
|---|---|---|
| Part modelling | Parametric sketches and features (OpenCascade kernel) | ✅ Available |
| Assembly | Parts placed with joints in Assembly Decks | ✅ Available |
| Manufacturing drawing | Views, dimensions, tolerances, title block | ✅ Available  |
| Stress analysis | Gmsh meshing, CalculiX solver, built-in result plots | ✅ Available |
| Thermal analysis | Heat and combined thermal–stress studies | ✅ Available  |
| Tolerances & fits | Process + tolerance class per part, interference and clearance at worst-case fits | ✅ Available |
| Manufacturability (DFM) | Checks for machining, casting, 3D printing 🚧 and plastic molding ✅ | 🚧 In development |
| Fatigue | Duty-cycle damage and life from multiple load cases | ✅ Available |
| Vibration analysis | Harmonic, FRF, Random vibration & Fatigue | 🗓️ Planned |
| Flow | Fluid & CFD | 🗓️ Planned |
| AI Assistant | Use mouse movements and voice commands together for 3D CAD | 🗓️ Planned |

## How it fits together

```
 Sketch ─► Part ─► Assembly ─► Drawing
              │          │
              └────► Mesh ─► Solve ─► Check ─► Results
                     (Gmsh)  (CalculiX)  (stress · heat · fatigue · fit · DFM)

          one model — a change anywhere updates everything
```

Analysis runs locally through a small helper on your own computer. Your models stay on your machine.

## Get started

- **Install:** download the latest bundle from the [KalpaXi releases](https://github.com/kalpaxi/kalpaxi/releases)
- **Read:** [documentation](https://github.com/kalpaxi/kalpaxi/wiki) · [examples](https://github.com/kalpaxi/kalpaxi/tree/main/examples)
- **Discuss:** [GitHub Discussions](https://github.com/kalpaxi/kalpaxi/discussions)
- **Report a bug:** [open an issue](https://github.com/kalpaxi/kalpaxi/issues)

## Contribute

KalpaXi welcomes engineers, developers, designers and testers.

- Good first issues are labelled [`good first issue`](https://github.com/kalpaxi/kalpaxi/labels/good%20first%20issue)
- Validation cases — hand calculations or test data compared with KalpaXi results — are especially valuable
- Please read `CONTRIBUTING.md` and agree to the Contributor License Agreement before your first pull request

## Licence

The KalpaXi core is free and open source under the **GNU AGPL v3**.
Third-party tools (OpenCascade, Gmsh, CalculiX, Three.js and others) keep their own licences — see `THIRD_PARTY_LICENSES`.

> **Engineering note:** KalpaXi helps you check designs; it does not replace engineering judgement.
> Results must be reviewed by a qualified engineer before they are used for real products.

---

<div align="center">

© 2026 The KalpaXi authors

</div>
