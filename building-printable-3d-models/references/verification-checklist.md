# Verification checklist

Read this checklist at the start of `STAGE_2_BUILD`. Perform manufacturing verification independently of modeling and retain evidence with the revision.

## Geometry and manufacturing verification

- Export STEP, re-import the STEP B-Rep, and confirm it is a valid solid. Compare exact bounds and solid count with the approved specification.
- Export 3MF in millimeters. Confirm its mesh is closed and manifold, object count is correct, and scale/orientation matches the validated manufacturing geometry.
- Probe or section-check wall/floor thickness, full-thickness stencil bridges, holes, countersinks, clearance, mating interfaces, and critical spans; confirm they meet the approved geometry and manufacturing limits.
- Run relevant tests and inspect both overall and local views after important visual changes. Do not treat a successful export as manufacturing validation.

## Preview, versions, and delivery

- Render the final PNG from the final manufacturing geometry used for the released STEP and 3MF. Reject a stale, mismatched, or different PNG.
- Preserve all prior versions and use a new revision identifier for every changed or delivered artifact; never silently overwrite an existing delivery.
- Deliver exactly one STEP, exactly one 3MF, and exactly one PNG as Final Deliverables 2. Include a delivery summary naming the revision, parameters/assumptions, independent manufacturing verification results, and any limits or follow-up checks.
