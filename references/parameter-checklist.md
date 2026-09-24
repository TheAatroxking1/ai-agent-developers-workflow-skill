# Parameter checklist

Read this checklist at the start of `STAGE_2_PARAMETERS`. Record the source of every value as user-provided, approved assumption, or manufacturing constraint.

## Common requirements

- Confirm overall dimensions: length, width, height, diameter, and reference datum. State millimeters only after telling the user that mm is the working default; convert any other stated unit explicitly.
- Confirm geometry and function: profile, radii, chamfers, draft, raised/recessed depth, orientation, load path, and accessible faces.
- Confirm material and print/manufacturing process: printer/process, material, nozzle or minimum feature, layer direction, support constraints, and finish.
- Confirm tolerance, mating features, assembly clearance, fasteners, hole type/diameter/position, countersink/counterbore, wall/floor thickness, and bridge/span limits.
- Do not guess overall dimensions, mating features, holes, thickness, safety-critical geometry, or other form/function-critical inputs. Stop and request clarification when they are unknown.

## Object-specific checks

| Object | Confirm before specification approval |
| --- | --- |
| Signs and stencils | Text, font, character size, character width, letter spacing, relief or cut-through geometry, minimum stroke, isolated islands, full-thickness connecting bridges, mounting method, and viewing face. |
| Plates and brackets | Plate thickness, bends or ribs, load direction, mounting-hole count/diameter/centers, edge distance, fasteners, clearance, and safety-critical strength geometry. |
| Enclosures | Overall envelope, wall thickness, internal keep-outs, PCB/connector datum, bosses, vents, lids, snaps/screws, cable exits, material, and thermal or electrical safety constraints. |
| Fitted parts | Counterpart measurement method, mating geometry, tolerance, clearance/interference target, insertion direction, load, retention, and trial-fit revision strategy. |
| Decorative models | Overall size, silhouette, minimum details, base/contact area, hollowing or drainage, orientation, material, and acceptable simplification. |

Mark every unresolved critical value as a blocker. Only user-authorized non-critical values may use a stated conservative printable default.
