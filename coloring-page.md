---
name: coloring-page
description: "Create clean, printable black-and-white coloring pages or color-by-number pages for Claire, Collins, or Judah. Use anytime the user asks for a coloring page, coloring sheet, or color-by-number page."
---
# Coloring Pages Generator

Specialized generator for printable, age-appropriate black-and-white coloring pages and color-by-number sheets designed for Claire, Collins, or Judah.

## Target Audience Profiles

- **Claire** (Default Audience): 4-year-old girl (DOB: 5/27/2022). Needs bold, clear outlines with moderate detail suitable for preschool coloring.
- **Collins**: 2-year-old girl (DOB: 10/9/2024). Needs very simple shapes, extra thick lines, large open spaces, and minimal clutter suitable for a toddler.
- **Judah**: 7-year-old boy (DOB: 6/1/2019). Judah has severe disabilities and only has use of left hand. Appropriate images will be targeted to a 2-year-old boy. Needs very simple shapes, extra thick lines, large open spaces, and minimal clutter.

If the user does not specify a child, default to **Claire**.

## Reference Images for Characters

When the prompt requests including one or more of the children, reference their photos stored in the skill resources:
- **Claire**: `assets/Claire1.jpg`, `assets/Claire2.jpg`
- **Collins**: `assets/Collins1.jpg`, `assets/Collins2.jpg`
- **Judah**: `assets/Judah1.jpg`, `assets/Judah2.jpg`

When generating an image depicting one of the children, pass the corresponding filenames in `image_references` and incorporate their visual likeness (hair, facial features) adapted into a black-and-white coloring book illustration.

## Core Rules & Output Specifications

1. **Format & Aspect Ratio**:
   - Designed for standard 8.5" x 11" paper.
   - Default aspect ratio: `3:4` or `4:5` (portrait orientation).
   - Use `4:3` or `5:4` (landscape) only when the scene is explicitly wide or horizontal.

2. **Strictly Black and White**:
   - Pure black line art on a clean white background.
   - **NEVER** color, shade, grayscale, crosshatch, or render gradients in the image.
   - Lines must be clean, crisp vector-style outlines.

3. **Color-by-Number Mode**:
   - Default is regular coloring page (NO numbers).
   - Only produce a color-by-number page when explicitly requested.
   - When requested:
     - Tag distinct bounded regions with numbers corresponding to up to 7 colors max.
     - Include a simple color key / legend at the bottom or top (e.g., 1 = Blue, 2 = Red, 3 = Green, etc.).
     - Do NOT include any numbers other than the color indicators and key.

4. **Age Appropriateness**:
   - Match line thickness and section sizes to the target child's developmental stage.