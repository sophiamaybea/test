# Stop Motion Lab — Reconstruction Packs

A GitHub index and reusable template for Stop Motion Engine dance reconstruction packs.

## Current dance

**Dance 2026-09-30**  
Active choreography: 00:09.0–01:00.5 · 51.5 seconds · 6 fps · 310 render frames.

[Open the complete asset pack in Google Drive](https://drive.google.com/drive/folders/1ED5xYioQyoIeoP0hdH8yDp6Lc1fZBr8o)

The Drive pack contains the complete renderer-ready assets: dance manifest, identity lock, camera/stage lock, 27-key-pose library, movement timeline, 310-frame index, 310 unique Grok prompts, onion-skin validation rules, and target identity/wardrobe images.

### Visual references

- [Identity close-up](https://drive.google.com/file/d/1UgW_EGQo7k2Yc1ciDYw4qy8jNJ0sTR6F/view)
- [Identity expression grid](https://drive.google.com/file/d/1w0nm50L3_IlTHxvRrYbGasuVyGGZiu58/view)
- [Wardrobe + body reference](https://drive.google.com/file/d/1kNFmWJnDZcwKhMJqDIuLBOp_Y8rKpT-7/view)

## Repository layout

```text
/
├── README.md
├── dances/
│   └── dance-2026-09-30/
│       ├── README.md
│       └── assets.json
└── template/
    ├── README.md
    ├── dance_manifest.template.json
    ├── assets.template.json
    └── renderer_contract.md
```

## Core rule

The source performance supplies **movement and timing only**. The target references supply identity, body, hair, wardrobe and appearance. Never inherit the source performer's identity.

Every rendered frame should be validated against the previous approved frame using the onion-skin continuity rules before advancing.
