---
name: rei-photo-album
description: Correct an uploaded photo using the exact @Rei face reference, then create nine distinct candid photos by default from the same session. Use for a ten-image square Rei album with strict body, outfit, and location continuity and a handheld iPhone Photo mode look.
---

# Rei Photo Album

## Use this skill

Attach the original photo and make the exact `@Rei` face reference available. In Codex, invoke `$rei-photo-album`. In ChatGPT, select the skill where supported or attach `SKILL.md` and ask ChatGPT to follow it. Example request:

> Use rei-photo-album with my attached original and @Rei. Create the full ten-photo album.

Use an image tool that accepts visual references and can reuse its output as an input. Resolve `@Rei` to the actual face reference available in the current session. If the mention cannot be resolved, ask for the exact reference image to be attached and identified as `@Rei`. If the original is missing, ask for it too. A name or text description alone cannot supply the face reference. If image editing or reference reuse is unavailable, explain what capability is needed and which outputs, if any, were completed.

Default to 10 photos total, with one corrected original and nine new candid moments. If the user specifies a total, count the corrected original as the first photo and generate enough new moments to reach that total.

Include “Compose and generate this image in a square 1:1 frame” in every image prompt, including the corrected original and all new photos.

## iPhone Photo mode realism

Apply these instructions to every generation prompt, including the correction.

- Keep the surroundings legible with natural softness in distant detail. Avoid Portrait mode blur, artificial bokeh, crunchy sharpening, clarity halos, and uniformly crisp microtexture across skin, fabric, foliage, and surfaces.
- Match the face, neck, and hands to the scene's light direction, color, and shadow falloff. Keep subtle pores and uneven skin tone where visible at the shot distance. Avoid beauty smoothing, added fill on the face, and lifting every shadow.
- Frame new moments like a friend reacting to an activity. Allow slight off-center framing, incidental overlaps, and props partly outside the frame. Show believable timing and movement. For falling grain, splashes, or moving animals, allow irregular spacing and slight motion softness where plausible.

## Rei’s beauty mark

In every prompt where her face may be visible, specify one small beauty mark on Rei’s anatomical right cheek, just below the outer corner of her right eye. It appears on the viewer’s left in the front-facing reference. Keep the mark on that same anatomical cheek as the camera angle changes. Omit it if that spot is hidden by the angle, hair, or a prop. Never mirror the mark, duplicate it, or place it on her left cheek.

Check the placement against the face reference before accepting each frame. Use her head orientation to identify the visible cheek. Flag any mirrored, duplicated, or misplaced mark during review.

## Stage 1 — Correct the original

Edit the uploaded image using the original for body proportions, outfit, and location, and `@Rei` for facial identity. Preserve Rei's recognizable facial features and geometry. Improve lighting, skin texture and tone, expression, hair, and shadows. Adjust the lighting and facial direction naturally where useful. Keep the original body proportions, outfit and accessories, and identifiable location intact.

Inspect the corrected image against both references before proceeding. Fix visible identity or continuity drift first. Keep the accepted correction as image 1 and use it as the master reference for all new frames.

## Stage 2 — Create distinct candid moments

Plan different activities that could happen in this location, using the surroundings and objects plausibly available there. Imagine a friend freely moving around and catching spontaneous moments. Give each frame a distinct activity, pose or movement, camera height and direction, shot scale, and placement in the frame. Compare the plan across all new frames and against image 1 to catch repeated compositions.

Generate the new frames separately. Use the same corrected master for each frame and the exact `@Rei` face reference wherever the face is visible. Preserve the character, body proportions, exact outfit and accessories, identifiable location, and general lighting conditions. Reconstruct the surroundings from each new camera position with consistent landmarks and spatial relationships. Create a new scene view for each frame. Crops, rotations, and slight rearrangements of the master do not qualify.

Favor scene-specific surprises. Try radically different viewpoints such as overhead, ground level, from behind, an oblique side angle, an extreme close-up, or a distant environmental view. Let Rei fall near the edge, face away, appear partially cropped or obscured, or leave the frame for a detail that still belongs to the session. Apply the same continuity checks wherever the relevant details are visible.

## Review and deliver

Review the full album together for the iPhone Photo mode look, visible `@Rei` identity, body and outfit continuity, and recognizable location. Check that the new frames differ in activity and composition. Check for uniform sharpness, a polished face that feels separate from the scene, and overly tidy action or framing. Report any visible issue by frame. Ask before using another generation to revise a completed frame.

Check the pixel dimensions of each image. If a frame comes back non-square, deliver it and report its dimensions. Ask before retrying so the user can control generation usage. Deliver the requested number of separate images in order. Put the corrected original first, followed by the new candid moments. If saving files, number them starting at 01. Each image should be available individually.
