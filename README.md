# Cmacc-app2
Rewriting and formalizing the Prose Object rendering engine

The goal is to work from first principles to at least one implementation that is reasonably fast and has the ability to tag each expansion span with metadata regarding its name and origin map.

In most condensed form:

1. Recursive expansion of {a Variable} in a string, by exactly matching the Variable's string with a key name in a Map and substituting the corresponding value for the variable string and escape characters;
2. Expansion of the Map by recursive expansion of referenced Maps.  Lazy, depth-first expansion.
3. With a optional "prefixing" notion for the references.  (This explanation requires expansion.)

The rendering engine should work with Maps stored in a number of formats, including the Prose Object ".md" format of the many repos at GitHub.com/CommonAccord.

The rendered documents should be identical in substance to those currently produced by Cmacc-app.

Additional functionality should be vigorously resisted except where absolutely convenient and consistent with the expansion notion.  (This explanation requires expansion.  Two examples are i)  solution the many /G/Z/ files and ii) a solution to resolving Map names when referencing a foreign set of Maps that have their own namespace.

