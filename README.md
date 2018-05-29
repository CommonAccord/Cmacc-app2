# Cmacc-app2
Rewriting and formalizing the Prose Object rendering engine

The goal is to work from first principles to at least one implementation that is reasonably fast and has the ability to tag each expansion span with metadata regarding its name and origin.

In most condensed form:

1. Recursive expansion of {variables} in a string, by substituting the value of a matching key in a map;
2. Expansion of the map by recursive expansion of referenced maps.  Lazy, depth-first.
3. With a "prefixing" notion for the references.  (This explanation requires expansion.)

The rendering engine should work with maps stored in a number of formats, including the Prose Object ".md" format of the many repos at GitHub.com/CommonAccord.

The rendered documents should be identical in substance to those currently produced by Cmacc-app.


