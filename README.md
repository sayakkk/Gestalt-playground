# Gestalt-playground
An interactive exploration of the Gestalt principles of perceptual organization. 

Laws of Gestalt — Interactive

⚠️ Work in progress. This is an active experiment, not a finished piece.

An interactive exploration of the Gestalt principles of perceptual organization. Built in the spirit of Laws of UX and userinterface.wiki — where abstract principles become tangible through direct manipulation.
What this is
A single-page web experiment that takes six classical Gestalt principles — formulated by Wertheimer, Köhler, and Koffka around 1912 — and turns each into a small interactive demonstration. The goal is for the reader to feel the principle take effect, not just read about it.
Current principles implemented:

Proximity — Same dots regroup into rows, columns, clusters, or scattered points depending on spacing.
Similarity — Shape, color, and size as independent grouping axes. Switch the axis, watch the groups reorganize.
Continuity — A single curve split into two pieces, each rotated to a random angle. Find the rotation that restores the original continuous flow.
Closure — Kanizsa figures (triangle, cube, star) at random initial rotations. Slide to find the alignment where an illusory shape emerges from nothing.
Figure & Ground — Three cues (convexity, layering order, size) for deciding what counts as figure.
Common Fate — Lasso dots into groups, assign each group a direction, then animate. The groups disappear into the crowd when motion stops.

Why "work in progress"
The implementation is intentionally exploratory. A few principles have gone through multiple redesigns because the right interaction for a given principle isn't obvious — and what reads as obvious on paper often fails in practice. For example:

The continuity demo went through three different framings before landing on the current "rotate two halves of a curve" version.
The closure demo's Kanizsa cube took several iterations to get the corner pac-men arrangement right (the canonical Kanizsa cube has a non-obvious structure where two diagonal corners show overlapping pac-men pairs while the other two corners show single pac-men).
The figure & ground demo is still the weakest — three cues feel disjointed and the "invert" interaction doesn't always make the perceptual shift dramatic enough.

The current version is best understood as a snapshot of an ongoing search for what makes a principle interactively legible, not a polished finished product. Some demos work well; others are still being figured out.
Things still being tried

More effective interactions for principles where the current demo feels weak (especially figure & ground)
Better visual hierarchy between the "what to do" instruction and the "what just happened" reveal
Tighter feedback loops (the speech-bubble reveal on alignment is one attempt at this)
Possibly: a few additional principles (Prägnanz, symmetry, common region)

Tech

Single static HTML file. No build step, no framework.
Vanilla JS, inline <style>, inline <script>.
SVG for all visual elements that need precise geometry (Kanizsa figures, continuity curves, arrows).
Plain HTML/CSS for the rest.

To run: open gestalt.html in a browser. That's it.
References

Wertheimer, M. (1923). Untersuchungen zur Lehre von der Gestalt II.
Koffka, K. (1935). Principles of Gestalt Psychology.
Köhler, W. (1947). Gestalt Psychology.
Palmer, S. E. (1999). Vision Science: Photons to Phenomenology.

License
Free to use, modify, fork. If you use it for something interesting, I'd love to know.
