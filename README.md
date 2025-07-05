
# Mixbox 3D Model Components

This repository contains 3D models of parts for a modular controller (e.g., an arcade **Mixbox** layout). This README documents the geometry, materials, and relationships between these parts.

## File Descriptions

- **Mixbox Layout Bottom.gltf**  
  A single mesh  representing the bottom panel of the Mixbox. This is a solid plate (~8 mm thick) with a curved-edge profile. .

- **Mixbox Layout Top.gltf**  
  One mesh  for the top panel or lid. This is a very thin sheet (≈1 mm thick) with a detailed outline, likely fitting over the bottom panel. It has many primitives to form its edges (e.g., button holes or contours).

- **Mixbox Top Arc Sheet.gltf**  
  One mesh  for an “arc sheet” component. This is another thin (≈1 mm) surface. Its name suggests it’s an overlay or curved face plate that attaches to the top.


## Dimensions and Structure

All parts share essentially the same XY footprint, with an approximate bounding box of **297 × 134 × H** mm. The exact dimensions are:

| Filename                   | Dimensions (L × W × H)   |
|----------------------------|-------------------------|
| Mixbox Layout Bottom.gltf   | 296.9 × 133.8 × 8.0 mm  | 
| Mixbox Layout Top.gltf      | 296.9 × 133.8 × 1.0 mm  | 
| Mixbox Top Arc Sheet.gltf   | 296.9 × 133.8 × 1.0 mm  |

### Details

- **Mixbox Layout Bottom:**  
  ~297 mm by 134 mm, ~8 mm thick. 40 primitives. Normals vary continuously around edges, indicating rounded or chamfered edges. A solid panel with curved borders.

- **Mixbox Layout Top:**  
  Same footprint, ~1.0 mm thick. 108 primitives. Complex outline with potential cutouts or bevels. Flat sheet with detailed edge geometry.

- **Mixbox Top Arc Sheet:**  
  Same footprint, ~1.0 mm thick. 56 primitives. Flat/curved overlay sheet matching bottom outline.



## Assembly Notes

- **Bottom Panel:** Base of the enclosure, provides structural support (8 mm thick).
- **Top Panel:** Sits above the bottom panel as the main cover or face; may include cutouts for controls.
- **Arc Sheet:** Thin overlay that aligns with Top Panel; provides a support to use your artwork.
- **Artwork:** The artwork file is in Assets folder. Please note change only background to your like.

👉 All parts align in the XY plane and stack vertically: **Bottom (thick base) → Top Panel → Arc Sheet**.

## Build Notes

- These layouts are standard **Mixbox-style** layouts.
- For right-hand-side movement key, simply flip the sheet after cuttings for a reversed Mixbox.
- If you don't want to use **Cherry MX low-profile switches**, you can use standard **Cherry MX buttons** (your choice).

### Recommended Components

- **Low Profile Keyswitch (Cherry MX Low Profile):**  
  [Buy here](https://meckeys.com/shop/accessories/keyboard-accessories/key-switches/cherry-low-profile-mechanical-switch/?attribute_pa_cherry-mx=red)

- **Standard Cherry MX Switches:**  
  [Buy here](https://meckeys.com/shop/accessories/keyboard-accessories/key-switches/cherry-mx-clear-top/)

- **Keycaps:**  
  [Blank DSA 1U Keycaps (Grey)](https://meckeys.com/shop/accessories/keyboard-accessories/keycaps/blank-dsa-keycaps-1u/?attribute_pa_variations=grey)

- **Standoffs and Screws:**  
  [Hex Standoffs](https://www.amazon.in/Immech-Pillar-Standoff-Hexagonal-Spacing/dp/B08CBD38W1)  
  [Matching Screws](https://amzn.in/d/87QF44h)

## Render Previews


- ![Mixbox Layout Bottom Render](https://github.com/VISHALBHARDWAJ123/mixbox_3d_model/blob/master/Assets/Bottom%20Layout.png)
- ![Mixbox Layout Top Render](https://github.com/VISHALBHARDWAJ123/mixbox_3d_model/blob/master/Assets/Top%20Layout.png)
- ![Mixbox Top Arc Sheet Render](https://github.com/VISHALBHARDWAJ123/mixbox_3d_model/blob/master/Assets/Top%20arc%20sheet.png)
- ![Mixbox Artwork Render](https://github.com/VISHALBHARDWAJ123/mixbox_3d_model/blob/master/Assets/Top%20Drawing%20for%20artwork.png)

