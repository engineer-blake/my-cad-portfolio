# CAD Portfolio: Michael Blakely

Mechanical design and drafting work across **Autodesk Inventor**, **FreeCAD** and **AutoCAD**, built around one product: a 100 mm bench vise, the bracket that mounts it, and the workshop cell that produces it.

| # | Project | Software | Files |
|---|---------|----------|-------|
| 1 | [Bench vise assembly](#1-bench-vise-assembly-inventor) | Autodesk Inventor | STEP |
| 2 | [Parametric mounting bracket](#2-parametric-mounting-bracket-freecad) | FreeCAD | FCStd, STEP |
| 3 | [Fabrication cell layout](#3-fabrication-cell-layout-autocad) | AutoCAD | DXF |

> Modelled from a reference design. The 3D models, parametric setup and layout drafting are my own work in each tool.

---

## 1. Bench vise assembly (Inventor)



A 9-part lead-screw bench vise: 100 mm jaw width, 80 mm maximum opening, Tr16×4 screw (4 mm jaw travel per handle turn).

**What's in it**
- Part models with Inventor Hole features (Tr16×4 and M5 threads) and Content Center fasteners (ISO 10642 M5)
- Constrained assembly checked for interference across the opening range

**Design decisions**
- The screw axis sits 25 mm above the base, below the jaw plates, so the screw never interferes with the clamping faces.
- The movable jaw runs on a 39.8 mm key in a 40 mm slideway (0.20–0.30 mm clearance). That's enough to slide freely without the jaw rocking.
- The jaw plates are separate hardened parts (50–55 HRC) held by countersunk screws, so worn faces are replaced instead of the whole jaw.
- Tolerancing scheme: the base underside is datum A and the fixed jaw face is datum B. The jaw face is perpendicular to A within 0.05 mm, and the slideway is parallel to A within 0.05 mm.

---

## 2. Parametric mounting bracket (FreeCAD)

A gusseted steel L-bracket that bolts the vise to a bench front or wall. It uses the vise's 210 × 90 mm M10 hole pattern.

**Spreadsheet-driven:** 16 aliased parameters (plate size, hole pattern, slot spacing, gussets, fillet) drive every sketch and feature. Changing 6 cells resizes it for a 125 mm vise with no sketch edits.

**Design decisions**
- The vise overhangs the leg, so two 8 mm gussets carry the bending load into the wall bolts.
- Slotted wall holes (13 × 30 mm) allow levelling, because bench and wall holes never line up exactly.
- The vise seat face is datum B, with flatness 0.1 mm, so the vise base seats without rocking.

---

## 3. Fabrication cell layout (AutoCAD)

An 8 × 6 m workshop for producing the vise, drawn at 1:40 on A3.

**Drafting setup:** 11-layer standard (walls, equipment, safety, flow, aisle, dimensions), equipment as attributed blocks with an extracted schedule, annotative dimensions, and a paper-space layout with a locked 1:40 viewport.

**Design decisions**
- Stock comes in through the roller door to the rack. Production then flows one way, saw → drill → fitting bench → weld bay → dispatch, without crossing itself.
- The weld bay is in the far corner and screened on both open sides, which keeps arc flash and spatter away from the aisle and bench.
- A 1200 mm main aisle stays clear end to end. Fire extinguishers sit at the exit and at the weld bay entry.

---

## Contact

**Michael Blakely**: [blakelymike08@gmail.com] ·

Open to mechanical design, CAD and engineering roles, including remote and part-time work.
