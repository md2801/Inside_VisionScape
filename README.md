# VisionScape — Turning Indoor Spaces into Intelligent Floorplans

**Live Demo:**
[Click Here to access website](https://md2801.github.io/Inside_VisionScape/)

---

## Overview

VisionScape is a scrollable, single-page web presentation documenting an AI research project that automatically converts indoor 3D scene data into structured 2D floorplans using deep learning. The page walks through the full research narrative — from the problem statement and system pipeline through to architecture design, experimental results, and future directions.

The presentation is built as a self-contained HTML file with a dark, cinematic visual style. It is intended to communicate technical depth clearly to both technical and non-technical audiences.

## Project Highlights

- Documents a hybrid CNN–Transformer architecture (RoomToFP v7) capable of predicting room polygons and dense structural masks simultaneously.
- Covers a full eight-version model evolution, showing what each architectural decision changed and why.
- Designed to be readable at a distance on a large display, with big typography and high-contrast visuals.
- Includes an animated architecture diagram with live data-flow visualisation built entirely in SVG and CSS.
- Fully self-contained — no build step, no dependencies, no server required.

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox, backdrop-filter, keyframe animations) |
| Interactivity | Vanilla JavaScript (IntersectionObserver, scroll events) |
| Typography | Google Fonts — Space Grotesk, Inter, JetBrains Mono |
| Graphics | Inline SVG (architecture diagram, animated data-flow, floorplan visuals) |

No external JavaScript libraries or frameworks are used.

## Page Sections

- **Challenge** — Explains why floorplan generation is slow, expensive, and difficult to scale, with an animated breakdown of the traditional workflow.
- **Our Approach** — Describes the VisionScape pipeline step by step, from 3D scene ingestion and Bird's Eye View generation through to post-processed SVG output.
- **Core Technology** — Details the RoomToFP v7 architecture: ResNet/FPN CNN encoder, Transformer encoder on p4, polygon decoder with room queries, and FPN U-Net mask decoder. Includes an annotated, animated SVG diagram.
- **Research Journey** — Horizontal scrollable timeline covering all eight model versions (V1–V8), with outcomes and key findings for each.
- **Detection Capabilities** — Summarises what the system detects: room instances, wall boundaries, door/window openings, room type labels, polygon geometry, and export formats.
- **Honest Science** — Transparent account of current limitations (polygon precision, opening detection, post-processing dependency) alongside concrete future research directions.

## Authors

Aaqil Irfan Modak · Monal Dangi · Siddhant Salgia
