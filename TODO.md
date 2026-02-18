# Logo Update Plan for ShopEasy

## Files to Edit:
1. **index.html** - Replace BOTH hero-logo AND nav-logo SVGs
2. **products.html** - Replace nav-logo SVG
3. **offers.html** - Replace nav-logo SVG
4. **about.html** - Replace nav-logo SVG
5. **register.html** - Replace nav-logo SVG
6. **contact.html** - Replace nav-logo SVG
7. **style.css** - Add CSS for new logo (optional - can be inline in each page)

## Changes per file:
- Replace old SVG code with new SVG logo
- Add CSS styling for `.shopeasy-logo` class
- Keep the same class names for nav-logo links

## New Logo SVG to use:
```
svg
<svg class="shopeasy-logo" viewBox="0 0 820 220" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="ShopEasy logo">
  <!-- Icon -->
  <g transform="translate(20,20)">
    <path class="bag" d="M60 60c0-16 13-29 29-29h72c16 0 29 13 29 29v96c0 22-18 40-40 40H100c-22 0-40-18-40-40V60z" />
    <path class="bag-shadow" d="M60 120c18 14 44 22 72 22s54-8 72-22v36c0 22-18 40-40 40H100c-22 0-40-18-40-40v-36z"/>
    <path class="handle" d="M92 52c0-20 16-36 36-36s36 16 36 36"/>
    <path class="bolt" d="M138 78l-26 40h22l-16 32 34-44h-22l8-28z"/>
  </g>
  <!-- Wordmark -->
  <g transform="translate(270,70)">
    <text class="wordmark" x="0" y="60" font-size="72" font-weight="800" font-family="Segoe UI, Inter, Arial, sans-serif" letter-spacing="-1">
      Shop<tspan fill="var(--primary)">Easy</tspan>
    </text>
    <text class="tagline" x="4" y="98" font-size="22" font-weight="600" font-family="Segoe UI, Inter, Arial, sans-serif">
      Smart shopping, made simple
    </text>
  </g>
</svg>
```

## CSS to add (can be in each file or in style.css):
```
css
<style>
  .shopeasy-logo{
    --primary:#1e88e5;
    --accent:#00c853;
    --dark:#0f172a;
    --muted:#94a3b8;
    width: 260px;
    height: auto;
    display: inline-block;
  }
  .shopeasy-logo .bag { fill: var(--primary); }
  .shopeasy-logo .bag-shadow { fill: rgba(15, 23, 42, 0.12); }
  .shopeasy-logo .handle { stroke: #ffffff; stroke-width: 10; fill: none; stroke-linecap: round; }
  .shopeasy-logo .bolt { fill: var(--accent); }
  .shopeasy-logo .wordmark { fill: var(--dark); }
  .shopeasy-logo .tagline { fill: var(--muted); }
  .shopeasy-logo:hover .bolt { filter: drop-shadow(0 4px 8px rgba(0,0,0,.18)); transform: translateY(-1px); }
  .shopeasy-logo .bolt { transition: .2s ease; transform-origin: center; }
</style>
```

## Status: PENDING APPROVAL
