# cat-space-balance

## Overview

`cat-space-balance` is a scalar function that evaluates the relationship between a cat and its surrounding space in a photograph. Every photograph of a cat is a negotiation between subject and environment — the borders of the frame define a small universe, and everything within them either serves the cat or distracts from it. This function scores how well that negotiation has been resolved, producing a value between 0 and 1 that reflects whether the surrounding space supports the cat or competes with it.

## Input

The function accepts a single required field:

| Field   | Type    | Required | Description |
|---------|---------|----------|-------------|
| `image` | `image` | Yes      | A photograph containing a cat. |

The image may be any photograph containing a cat — a carefully composed portrait or a hasty phone snapshot, indoors or outdoors, minimal or rich. The function does not evaluate technical image quality (sharpness, exposure, resolution). It evaluates only the compositional relationship between the cat and the space around it.

## Output

A scalar score between **0** and **1**:

- **Scores near 1.0** indicate that the surrounding space supports the cat without competing. The cat is the clear focal point, the framing feels inevitable, and the environment complements the subject in quiet partnership. The frame could not have been drawn any other way.
- **Scores near 0.5** indicate a mixed result. The cat is present as a subject but the surrounding space introduces imperfections — moderate background distractions, slightly loose or tight framing, or environmental elements that partially compete with the subject.
- **Scores near 0.0** indicate that the environment overwhelms, suffocates, or marginalizes the cat. The subject is lost in visual clutter, dwarfed by an overly wide frame, trapped by an overly tight crop, or reduced to a bystander in its own photograph.

## Use Cases

- **Pet owners** sharing photos on social media who want their cat to be the undeniable star of the image, not a small shape lost in a cavernous room.
- **Animal shelter volunteers** photographing cats for adoption listings, where each animal needs to feel present and approachable, framed in a way that invites connection rather than confusion.
- **Photographers** curating portfolios of animal work who want every composition to feel intentional and inevitable.
- **Content platforms** that surface or rank cat photography and want a principled, consistent measure of compositional quality.
- **Photo editing tools** that suggest crops or framing adjustments to improve the balance between subject and surroundings.

## What It Evaluates

The function assesses three interdependent qualities of the input image. Each quality is scored independently and contributes equally to the final result.

### 1. Visual Hierarchy

Does the cat sit at the apex of the composition's visual hierarchy? The eye should arrive at the cat first and return to it naturally after wandering. The surrounding space — a stretch of hardwood floor, a rumpled duvet, an expanse of sky — should recede and feel secondary. The background should be quiet while the cat is loud, not through sharpness or saturation alone, but through the compositional logic of the frame itself.

**Scores high when:** Every part of the frame knows its place. The space understands it is there to support, not to perform. The cat advances and the world behind it falls away.

**Scores low when:** Busy backgrounds with colorful or patterned elements pull the eye sideways. Competing objects fracture attention so the cat becomes one element among many rather than the reason the photograph exists.

### 2. Spatial Proportion

Does the amount of the frame the cat occupies relative to the surrounding space feel natural and inevitable? There is no single correct ratio — a cat perched on a vast, snow-covered field can be compositionally perfect even though it occupies a small fraction of the image, provided the emptiness is purposeful. Equally, a tight crop can succeed if the cat does not feel pressed against the edges.

**Scores high when:** The cat has been given exactly the space it needs, no more and no less. The proportion feels deliberate and considered, as though the photographer understood intuitively how much world the cat needed around it.

**Scores low when:** The frame is so wide that the cat shrinks into insignificance and becomes an incidental detail, or the crop is so tight that the cat feels trapped and confined against the borders of the image.

### 3. Environmental Harmony

Does the content of the surrounding space complement the cat's presence or undermine it? The space surrounding a cat is never truly empty — it is filled with context. A sunlit patch of carpet tells us something about the warmth of the moment. A cluttered countertop tells us something too, though perhaps something less flattering to the composition.

**Scores high when:** The environment provides mood and context — the coziness of a blanket, the openness of a garden, the calm geometry of a windowsill — without demanding close study or stealing focus. The setting feels like a place the cat belongs, and the environment tells a quiet story that begins and ends with the subject.

**Scores low when:** Visual noise from cluttered objects, competing patterns, or colors that bear no relationship to the cat fill the surrounding space. The cat is reduced from protagonist to bystander. The setting and the cat feel like strangers sharing an awkward frame.

## Scoring Philosophy

The highest scores belong to images where all three qualities converge: where the cat is the clear focal point, where the surrounding space is proportioned with intuitive rightness, and where the environment supports the subject in quiet, purposeful partnership. In such photographs, the frame feels as though it could not have been drawn any other way. The cat has exactly the space it needs, and the space knows exactly what it is there to do.