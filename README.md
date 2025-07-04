
# Mixbox 3D Model Components

This repository contains 3D models of parts for a modular controller (e.g., an arcade **Mixbox** layout). Each model was exported from **Onshape (glTF 2.0)** and contains one mesh under a single node. This README documents the geometry, materials, and relationships between these parts.

## File Descriptions

- **Mixbox Layout Bottom.gltf**  
  A single mesh (`mesh0_mesh`, Node `Part 1`) representing the bottom panel of the Mixbox. This is a solid plate (~8 mm thick) with a curved-edge profile. The mesh is split into multiple primitives (triangles) to capture its shape.

- **Mixbox Layout Top.gltf**  
  One mesh (`mesh0_mesh`, Node `Part 1`) for the top panel or lid. This is a very thin sheet (≈1 mm thick) with a detailed outline, likely fitting over the bottom panel. It has many primitives to form its edges (e.g., button holes or contours).

- **Mixbox Top Arc Sheet.gltf**  
  One mesh (`mesh0_mesh`, Node `Part 1`) for an “arc sheet” component. This is another thin (≈1 mm) surface that matches the bottom panel’s outline. Its name suggests it’s an overlay or curved face plate that attaches to the top. The mesh geometry is similarly subdivided to represent curved edges.

Each file’s scene graph has one root node (`Root` scene) with a single child node named `Part 1`, which references `mesh 0`. There are no additional nodes or hierarchy levels (no nested nodes).

## Dimensions and Structure

All parts share essentially the same XY footprint, with an approximate bounding box of **297 × 134 × H** mm. The exact dimensions are:

| Filename                   | Dimensions (L × W × H)   | Meshes | Materials |
|----------------------------|-------------------------|--------|-----------|
| Mixbox Layout Bottom.gltf   | 296.9 × 133.8 × 8.0 mm  | 1      | 1         |
| Mixbox Layout Top.gltf      | 296.9 × 133.8 × 1.0 mm  | 1      | 1         |
| Mixbox Top Arc Sheet.gltf   | 296.9 × 133.8 × 1.0 mm  | 1      | 1         |

### Details

- **Mixbox Layout Bottom:**  
  ~297 mm by 134 mm, ~8 mm thick. 40 primitives. Normals vary continuously around edges, indicating rounded or chamfered edges. A solid panel with curved borders.

- **Mixbox Layout Top:**  
  Same footprint, ~1.0 mm thick. 108 primitives. Complex outline with potential cutouts or bevels. Flat sheet with detailed edge geometry.

- **Mixbox Top Arc Sheet:**  
  Same footprint, ~1.0 mm thick. 56 primitives. Flat/curved overlay sheet matching bottom outline.

## Materials and Textures

Each model uses a single **PBR material**:

- **Base Color:** `[0.6157, 0.8118, 0.9294, 1.0]` (light blue)
- **Metallic:** `0.0` (non-metallic)
- **Roughness:** default (likely `1.0`)
- **Double-Sided:** `true`
- **Textures:** None (no UV textures referenced)

All primitives use this single material uniformly.

## Assembly Notes

- **Bottom Panel:** Base of the enclosure, provides structural support (8 mm thick).
- **Top Panel:** Sits above the bottom panel as the main cover or face; may include cutouts for controls.
- **Arc Sheet:** Thin overlay that aligns with the bottom panel; could provide curvature or support beneath/above the top panel.

👉 All parts align in the XY plane and stack vertically: **Bottom (thick base) → Top Panel → Arc Sheet**.

## Render Previews

*(Placeholder for renders – add images as needed)*

- ![Mixbox Layout Bottom Render](path/to/bottom_render.png)
- ![Mixbox Layout Top Render](path/to/top_render.png)
- ![Mixbox Top Arc Sheet Render](path/to/arc_render.png)

## License

> **⚠ No license information is provided.**  
> Assume **all rights reserved** unless otherwise stated. Please verify the original source for proper usage permissions.
