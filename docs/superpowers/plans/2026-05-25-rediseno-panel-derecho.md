# Rediseno Panel Derecho Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Convert the right-side info panel into a more visual, ad-style product presentation without breaking gallery behavior.

**Architecture:** Keep the existing single-file HTML structure, replace the current long-description area with structured marketing blocks, and extend the item data model so the tower can render richer feature cards while machines and videos continue to work safely. Preserve the current gallery selection logic and contact area.

**Tech Stack:** Static HTML, CSS, vanilla JavaScript

---

### Task 1: Restructure The Right Panel Markup

**Files:**
- Modify: `C:\Users\Bafer\OneDrive\maqueta petrolera\index.html`

- [ ] Replace the current description-only block with a visual content stack: eyebrow, title, price, trait line, short intro, benefits list, material card, and functionality card grid.
- [ ] Keep the specs grid and contact card below the new visual content so pricing, dimensions, delivery, and WhatsApp remain accessible.

### Task 2: Add Styling For The New Marketing Layout

**Files:**
- Modify: `C:\Users\Bafer\OneDrive\maqueta petrolera\index.html`

- [ ] Add CSS for the new hero text, benefits rows, material highlight card, and three-image functionality grid.
- [ ] Update the responsive rules so the new blocks still fit on tablet and mobile widths.

### Task 3: Extend Data And Rendering Logic

**Files:**
- Modify: `C:\Users\Bafer\OneDrive\maqueta petrolera\index.html`

- [ ] Extend the tower data with structured marketing content and image cards using existing photos from `fotos/`.
- [ ] Add safe fallback rendering for machines and videos so the same panel can render shorter generic content when those items are selected.
- [ ] Update `selectItem()` to fill the new fields and toggle the functionality card section when there is no image-card content.

### Task 4: Verify The Final Flow

**Files:**
- Modify: `C:\Users\Bafer\OneDrive\maqueta petrolera\index.html`

- [ ] Verify the HTML still loads from the local file path and through the local server.
- [ ] Verify that selecting a tower keeps the richer visual panel and that selecting machine/video items does not leave stale tower-only cards visible.
