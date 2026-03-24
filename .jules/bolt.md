## 2026-03-24 - Docusaurus Static Homepage Analysis
**Learning:** The Docusaurus homepage in this repository is entirely static. Attempts to optimize it via `React.memo()` or context prop-drilling provide zero measurable performance benefit and represent premature micro-optimization.
**Action:** Always verify if a site or page is statically generated before attempting React-specific runtime optimizations. Do not attempt to optimize without a genuine bottleneck.

## 2024-03-24 - Docusaurus Static Site Images
**Learning:** For statically generated Docusaurus sites, performance gains come from build optimization, asset preloading, and lazy loading strategies rather than React render optimizations. Inline SVGs don't support `loading="lazy"`.
**Action:** When working with Docusaurus, prioritize asset-level and build-level optimizations over component-level runtime micro-optimizations.
