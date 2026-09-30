# Renderer Contract

## Inputs

The renderer receives the asset map, reconstruction data, target identity references and previous approved frame. It must not require the original source video.

## Hard locks

- Target identity
- Target body proportions
- Wardrobe
- Static camera geometry
- Stage/environment
- Anatomy
- No source-performer identity leakage

## Frame execution

Render in ascending frame order. For frame N > 1, use frame N-1's approved render as the strongest continuity reference. Use the frame-specific prompt and interpolation data to introduce only the movement required for the next frame.

## Onion-skin gate

Overlay the candidate frame against the previous approved frame at approximately 35–50% opacity. Check center of mass, support contacts, joint paths, face stability, hair inertia, clothing inertia, screen position and camera geometry.

If a frame fails, regenerate that frame only. Do not advance until it passes.
