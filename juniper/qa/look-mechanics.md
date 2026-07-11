# Juniper Look Mechanics

Juniper looks around as a grounded fox, not as a rotating toy. The feet, lower torso, baseline, body scale, and tail root stay anchored. The amber eyes lead each gaze; the muzzle and head follow with restrained yaw or pitch; the ears reinforce the direction; the scarf tip and cyan-marked tail lag subtly without changing attachment or side.

## Motion budget

Each 22.5-degree step moves the pupils, muzzle, head, and ears by an even small amount. The torso changes only enough to support a natural head turn. No neighboring pair may introduce a large bend, scale change, baseline shift, tail jump, scarf flip, or silhouette snap.

## Cardinal pose families

- `000 up`: pupils sit high in the amber eyes; muzzle tips slightly upward; chin lifts; both inner ears remain visible and angle attentively upward; chest stays front-facing; scarf and tail remain anchored.
- `090 screen-right`: pupils and nose tip move to the image's right of head center; Juniper turns the head toward screen-right, revealing more of the left cheek and left side of the scarf while the far cheek and far ear become slightly occluded; tail follows only slightly.
- `180 down`: pupils sit low; muzzle and chin tuck toward the chest; upper eyelids and brow reinforce downward attention; ear tips relax slightly outward; feet, torso, scarf knot, and tail root remain fixed.
- `270 screen-left`: pupils and nose tip move to the image's left of head center; Juniper turns the head toward screen-left, revealing more of the right cheek and right side of the scarf while the far cheek and far ear become slightly occluded; tail follows only slightly.

## Intermediate directions

Diagonals interpolate the adjacent cardinal families without mirroring or independently re-centering cells. Eyes move first, then head and muzzle, then ears; the scarf tip and tail have restrained continuous follow-through. The `157.5 -> 180` and `337.5 -> 000` boundaries must each be exactly one natural step with no registration jump.

## Identity and physical constraints

Preserve the original amber eye construction, midnight-blue head and body, pale muzzle, pointed ear geometry, graphite scarf, and cyan tail markings. Do not add eye whites, googly pupils, extra markings, props, effects, labels, shadows, or whole-sprite rotation. The scarf stays worn around the neck and the tail remains attached at the same root in every pose.
