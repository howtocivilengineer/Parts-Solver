# Parts Solver

Build reusable civil engineering parts from a string — roads, kerbs, channels, walls, pads and more.

Parts Solver is a free, browser-based tool for building and reviewing layered civil engineering sections. Draw a part, define its layers, set the attach point and daylight, and see the result immediately in plan and 3D.

It is designed to sit alongside the other How To Civil Engineer tools — particularly Grading Solver — as a lightweight way to create the typical building blocks used in light-civils design.

### ▶ Run it now

**[Launch Parts Solver](https://howtocivilengineer.github.io/Parts-Solver/)**

Open the link and start building a part. Nothing needs to be installed and your work stays in your browser.

---

## Video walkthrough

*Coming soon.*

---

## What it does

Parts Solver lets you create a civil engineering part from a simple editable section.

There are two main types:

* **Horizontal** — open profiles for roads, footpaths, pads, berms, swales and similar surfaces. Layers follow the profile vertically below the finished surface.
* **Vertical** — closed sections for kerbs, channels and retaining walls. Additional layers can be added as parametric footings below the main section.

### Build the section

* Start from a built-in part such as a pavement, kerb, channel, berm or retaining wall.
* Drag vertices to change the geometry.
* Drag a segment to move it.
* Drag a midpoint to insert a new vertex.
* Add or remove vertices to create the section you need.
* Mirror a part for the opposite side of a road.
* Name the part and give it a code and colour.

### Add construction layers

Horizontal parts can be built up from multiple material layers such as:

* Wearing surface
* Basecourse
* Subbase
* Topsoil

Each layer can be given its own depth and follows the shape of the surface above it.

Vertical parts can use additional parametric layers with a depth and front/back projection — useful for foundation courses, bedding and wall blinding.

### Attach and daylight

The **Attach** point pins the part to the string and becomes the origin of the part.

The **Daylight** point defines where the part hands over to the earthworks.

A second daylight can be enabled when a part needs to run out in both directions — for example, a pavement attached at the centre of a road.

The string stays fixed; the part moves around its attach point.

### Control exposed faces

Layer 1 represents the exposed part.

Faces can be left on their automatic setting or manually switched between exposed and hidden. This gives control over which parts of a section are visible and which are buried.

### Check the geometry

Parts Solver provides live checks while you edit.

It warns about:

* Sections that double back
* Self-intersecting outlines
* Exposed overhangs
* Faces that cannot form a meaningful earthworks transition

The tool also reports the current width, depth, number of layers, total section quantity and exposed length.

### See it in 2D and 3D

The main view gives you an editable engineering section with:

* Dimensions
* Grid
* String and daylight markers
* Grades
* Face names
* Layer geometry

An orbitable 3D view shows the part swept along a 1 m run, making it easier to check the section as a three-dimensional object.

---

## Built-in parts

The current library includes:

| Category   | Parts                       |
| ---------- | --------------------------- |
| Horizontal | Pavement                    |
| Horizontal | Pavement — single slope     |
| Horizontal | Berm / swale                |
| Vertical   | Kerb — barrier              |
| Vertical   | Kerb — mountable            |
| Vertical   | Kerb and channel            |
| Vertical   | Dish channel                |
| Vertical   | Retaining wall — L          |
| Vertical   | Retaining wall — cantilever |

These are starting points rather than fixed templates. Edit the geometry, layers, attachment and daylight to create the section you need.

---

## The workflow

The panel follows the way you actually build a part:

**1 · Part**

Choose Horizontal or Vertical, select a starting part, then set its name, code, colour and mirror option.

**2 · Section**

Edit the section geometry by dragging vertices, segments and midpoints.

**3 · Layers**

Add construction layers and set their names and depths.

**4 · Attach & daylight**

Choose where the part attaches to the string and where it daylights into the earthworks.

**5 · Faces**

Review which Layer 1 faces are exposed and override the automatic result where required.

The result is shown immediately in the drawing and 3D views.

---

## Save and reopen parts

Parts Solver saves parts as `.json` files.

A saved part contains the geometry, layers, attachment and daylight positions, exposed faces, dimensions and other information required to reopen the part.

You can:

* **Save part** to create a JSON part file.
* **Open** a saved part.
* Drag a saved `.json` part onto the page to review it.

The saved format is designed around the Parts Solver model rather than being a generic CAD exchange format.

---

## Undo and redo

Full undo and redo are available while editing.

* **Ctrl + Z** — Undo
* **Ctrl + Shift + Z** — Redo
* **Ctrl + Y** — Redo

A complete drag/edit is treated as a single undo step, rather than recording every mouse movement.

---

## Privacy

Parts Solver runs entirely in your browser.

Your part geometry and saved files are not uploaded to a server for processing. The application is a single HTML page and the part data is handled locally in the browser.

---

## Run it locally / self-host

The tool is built as a standalone HTML application.

You can download the `index.html` file and open it directly in a modern browser, or host it on GitHub Pages or another static web host.

No server, database or build system is required.

---

## Tech

Parts Solver is built with:

* HTML
* CSS
* Vanilla JavaScript
* HTML Canvas

There are no frameworks or package installations required. The section geometry, layer calculations, validation, 2D drawing, 3D view and JSON save/load all run client-side.

---

## Part of the Solver set

Parts Solver is part of the browser-based civil engineering tools from **How To Civil Engineer**.

* **[TOPO Solver](https://github.com/howtocivilengineer/Topo-Solver)** — build and review a ground surface from survey points.
* **[Grading Solver](https://github.com/howtocivilengineer/Grading-Solver)** — develop pads, grades, batters and earthworks designs.
* **[Volume Solver](https://github.com/howtocivilengineer/Volume-Solver)** — compare surfaces and calculate cut and fill.
* **Parts Solver** — build the reusable civil engineering parts that make up a design.

The aim is the same across the set: useful civil engineering tools that are fast, free and available directly in the browser.

---

## Feedback

Found a bug, have an unusual section that does not work, or have an idea for another useful part?

Open an issue and describe what you were trying to build.

Screenshots or a saved Parts Solver `.json` file can be particularly useful when reporting a geometry problem.

---

## Disclaimer

Parts Solver is provided as an engineering aid. It does not replace professional engineering judgement, detailed design checks, construction drawings or certified engineering software.

Always verify dimensions, geometry, material depths, daylight conditions and other outputs against your own calculations and the requirements of the project before using them for design or construction.

No guarantee is provided that the software is free from errors or suitable for any particular project.

Use of Parts Solver is at your own risk. The developer accepts no responsibility for losses, damages or consequences arising from its use.

---

Built for civil engineers, surveyors and designers who want a fast, free way to build and review the everyday parts that make up a civil engineering design — without requiring a large desktop package.
