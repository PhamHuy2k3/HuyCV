## 2026-03-25 - Docusaurus Static Homepage Anti-Pattern
**Learning:** The Docusaurus homepage in this repository is entirely static. Wrapping components in `React.memo()` or prop-drilling context provides zero measurable performance benefit and should be avoided as premature micro-optimization.
**Action:** Do not attempt to add `React.memo()` or similar micro-optimizations to static Docusaurus pages, as they do not address any actual performance bottleneck and only add unnecessary complexity.
