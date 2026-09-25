# Trammel of Archimedes — CAD Capstone

Portfolio project for the Project Lead The Way *Introduction to Engineering
Design* course, QHS/PLTW IED Block C, fall 2024. Drawings checked by the course
instructor, revision B, 6 December 2024. Modeled in Autodesk Fusion.

## The mechanism

A trammel of Archimedes converts rotation into two perpendicular linear motions.
Two sliders travel in slots set at right angles; a rigid arm is pinned to both.
Any point on that arm traces an ellipse, and the semi-axes of that ellipse equal
the distances from the point to each of the two pivots.

This is what makes the device interesting to model: the shape of the traced
curve is not built into any surface. It is set entirely by two distances along
the handle, and the holes along the arm let the operator change it.

## Parts

Seven unique parts, ten instances. STL files render directly in GitHub's 3D
viewer, so any part can be rotated in the browser without downloading anything.
STEP files carry the exact solid geometry and open in any CAD system.

| Part | Qty | Drawing | STEP | STL |
|---|---|---|---|---|
| Assembly | — | [PDF](Toy%20Assembly/Trammel%20Toy%20Assembly%20Drawing.pdf) | [STEP](Toy%20Assembly/Trammel%20Toy%20Assembly.step) | [STL](Toy%20Assembly/Trammel%20Toy%20Assembly.stl) |
| Baseplate | 1 | [PDF](Baseplate/Baseplate%20Drawing.pdf) | [STEP](Baseplate/Baseplate.step) | [STL](Baseplate/Baseplate.stl) |
| T1 Block | 1 | [PDF](T1-Block%20Component/Trammel%20T1%20Component.pdf) | [STEP](T1-Block%20Component/Trammel%20T1%20Component.step) | [STL](T1-Block%20Component/Trammel%20T1%20Component.stl) |
| T2 Block | 2 | [PDF](T2-Block%20Component/Trammel%20T2%20Component.pdf) | [STEP](T2-Block%20Component/Trammel%20T2%20Component.step) | [STL](T2-Block%20Component/Trammel%20T2%20Component.stl) |
| T3 Block | 1 | [PDF](T3-Block%20Component/T3-Block%20Component.pdf) | [STEP](T3-Block%20Component/T3-Block%20Component.step) | [STL](T3-Block%20Component/T3-Block%20Component.stl) |
| Pin Slider Block | 1 | [PDF](Pin%20Slider%20Block/Pin%20Slider%20Block%20Drawing.pdf) | [STEP](Pin%20Slider%20Block/Pin%20Slider%20Block.step) | [STL](Pin%20Slider%20Block/Pin%20Slider%20Block.stl) |
| Screw Slider Block | 1 | [PDF](Screw%20Slider%20Block/Screw%20Slider%20Block%20Drawing.pdf) | [STEP](Screw%20Slider%20Block/Screw%20Slider%20Block.step) | [STL](Screw%20Slider%20Block/Screw%20Slider%20Block.stl) |
| Handle | 1 | — | [STEP](Handle/Handle.step) | [STL](Handle/Handle.stl) |
| Pin | 1 | — | [STEP](Pin%20block/Pin.step) | [STL](Pin%20block/Pin%20block.stl) |
| Screw | 1 | — | [STEP](Screw%20block/Screw%20block.step) | [STL](Screw%20block/Screw%20block.stl) |

The assembly drawing includes an exploded view and the full parts list.
The native Fusion archive, which holds the joints that make the mechanism move,
is here: [Trammel Toy Assembly.f3z](Toy%20Assembly/Trammel%20Toy%20Assembly.f3z).

## Design notes

Dimensions are imperial. The baseplate is 4.25 in square; wall thicknesses and
bores are inch fractions and decimals throughout.

Threads are modeled as cosmetic features over plain cylindrical geometry. Mated
threaded parts therefore overlap in the assembly — that overlap is the thread
engagement, not an interference fit.

Drawings were not produced for the handle, pin, and screw. These are simple
parts of primitive geometry; their dimensions can be read from the mating
parts' drawings or taken directly from the STEP files.

Component names in the assembly tree reflect the modeling history rather than
the part names used in the drawings — some parts appear as nested components of
the baseplate with working names. The parts list on the assembly drawing is the
authoritative reference.

## Files

STEP and STL are static geometry in one position. The joints exist only in the
Fusion archive.
