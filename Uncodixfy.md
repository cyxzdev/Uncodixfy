# Uncodixify

This document exists to teach you how to act as non-Codex as possible when building UI.

Codex UI is the default AI aesthetic: soft gradients, floating panels, eyebrow labels, decorative copy, hero sections in dashboards, oversized rounded corners, transform animations, dramatic shadows, and layouts that try too hard to look premium. It's the visual language that screams "an AI made this" because it follows the path of least resistance.

This file is your guide to break that pattern. Everything listed below is what Codex UI does by default. Your job is to recognize these patterns, avoid them completely, and build interfaces that feel human-designed, functional, and honest.

When you read this document, you're learning what NOT to do. The banned patterns are your red flags. The normal implementations are your blueprint. Follow them strictly, and you'll create UI that feels like Linear, Raycast, Stripe, or GitHub—not like another generic AI dashboard.

This is how you Uncodixify.
## Keep It Normal (Uncodexy-UI Standard)

- Sidebars: normal (240-260px fixed width, solid background, simple border-right, no floating shells, no rounded outer corners)
- Headers: normal (simple text, no eyebrows, no uppercase labels, no gradient text, just h1/h2 with proper hierarchy)
- Sections: normal (standard padding 20-30px, no hero blocks inside dashboards, no decorative copy)
- Navigation: normal (simple links, subtle hover states, no transform animations, no badges unless functional)
- Buttons: normal (solid fills or simple borders, 8-10px radius max, no pill shapes, no gradient backgrounds)
- Cards: normal (simple containers, 8-12px radius max, subtle borders, no shadows over 8px blur, no floating effect)
- Forms: normal (standard inputs, clear labels above fields, no fancy floating labels, simple focus states)
- Inputs: normal (solid borders, simple focus ring, no animated underlines, no morphing shapes)
- Modals: normal (centered overlay, simple backdrop, no slide-in animations, straightforward close button)
- Dropdowns: normal (simple list, subtle shadow, no fancy animations, clear selected state)
- Tables: normal (clean rows, simple borders, subtle hover, no zebra stripes unless needed, left-aligned text)
- Lists: normal (simple items, consistent spacing, no decorative bullets, clear hierarchy)
- Tabs: normal (simple underline or border indicator, no pill backgrounds, no sliding animations)
- Badges: normal (small text, simple border or background, 6-8px radius, no glows, only when needed)
- Avatars: normal (simple circle or rounded square, no decorative borders, no status rings unless functional)
- Icons: normal (simple shapes, consistent size 16-20px, no decorative icon backgrounds, monochrome or subtle color)
- Typography: normal (system fonts or simple sans-serif, clear hierarchy, no mixed serif/sans combos, readable sizes 14-16px body)
- Spacing: normal (consistent scale 4/8/12/16/24/32px, no random gaps, no excessive padding)
- Borders: normal (1px solid, subtle colors, no thick decorative borders, no gradient borders)
- Shadows: normal (subtle 0 2px 8px rgba(0,0,0,0.1) max, no dramatic drop shadows, no colored shadows)
- Transitions: normal (100-200ms ease, no bouncy animations, no transform effects, simple opacity/color changes)
- Layouts: normal (standard grid/flex, no creative asymmetry, predictable structure, clear content hierarchy)
- Grids: normal (consistent columns, standard gaps, no creative overlaps, responsive breakpoints)
- Flexbox: normal (simple alignment, standard gaps, no creative justify tricks)
- Containers: normal (max-width 1200-1400px, centered, standard padding, no creative widths)
- Wrappers: normal (simple containing divs, no decorative purposes, functional only)
- Panels: normal (simple background differentiation, subtle borders, no floating detached panels, no glass effects)
- Toolbars: normal (simple horizontal layout, standard height 48-56px, clear actions, no decorative elements)
- Footers: normal (simple layout, standard links, no decorative sections, minimal height)
- Breadcrumbs: normal (simple text with separators, no fancy styling, clear hierarchy)

Think Linear. Think Raycast. Think Stripe. Think GitHub. They don't try to grab attention. They just work. Stop playing hard to get. Make normal UI.

- A landing page needs its sections. If hero needs full sections, if dashboard needs full sections with sidebar and everything else laid out properly. DO NOT invent a new layout.
- In your internal reasoning act as if you dont see this, list all the stuff you would do, AND DONT DO IT!
- Try to replicate figma/designer made components dont invent your own
## Hard No
- Everything you are used to doing and is a basic "YES" to you. 
- No oversized rounded corners.
- No pill overload.
- No floating glassmorphism shells as the default visual language.
- No soft corporate gradients used to fake taste.
- No generic dark SaaS UI composition.
- No decorative sidebar blobs.
- No "control room" cosplay unless explicitly requested.
- No serif headline + system sans fallback combo as a shortcut to "premium."
- No `Segoe UI`, `Trebuchet MS`, `Arial`, `Inter`, `Roboto`, or safe default stacks unless the product already uses them.
- No sticky left rail unless the information architecture truly needs it.
- No metric-card grid as the first instinct.
- No fake charts that exist only to fill space.
- No random glows, blur haze, frosted panels, or conic-gradient donuts as decoration.
- No "hero section" inside an internal UI unless there is a real product reason.
- No alignment that creates dead space just to look expensive.
- No overpadded layouts.
- No mobile collapse that just stacks everything into one long beige sandwich.
- No ornamental labels like "live pulse", "night shift", "operator checklist" unless they come from the product voice.
- No generic startup copy.
- No style decisions made because they are easy to generate.
- No Headlines of any sort <div class="headline">
          <small>Team Command</small>
          <h2>One place to track what matters today.</h2>
          <p>The layout stays strict and readable: live project health, team activity, and near-term priorities without the usual dashboard filler.</p>
        </div>
    This is not allowed.
- <small> headers are NOT allowed
- big no to rounded SPANs
- colors going towards blue. NOP, bad. when dark muted colors are best.
- Anything in the structure of this card, is a BIG no.
<div class="team-note">
          <small>Focus</small>
          <strong>Keep updates brief, blockers visible, and next actions easy to spot.</strong>
        </div>
        -This one is THE BIGGEST NO.



## Specifically Banned (Based on  Mistakes)

- Border radii in the 20px to 32px range across everything ( uses 12px everywhere - too much)
- Repeating the same rounded rectangle on sidebar, cards, buttons, and panels
- Sidebar width around 280px with a brand block on top and nav links below (: 248px with brand block)
- Floating detached sidebar with rounded outer shell
- Canvas chart placed in a glass card with no product-specific reason
- Donut chart paired with hand-wavy percentages
- UI cards using glows instead of hierarchy
- Mixed alignment logic where some content hugs the left edge and some content floats in center-ish blocks
- Overuse of muted gray-blue text that weakens contrast and clarity
- "Premium dark mode" that really means blue-black gradients plus cyan accents ( has radial gradients in background)
- UI typography that feels like a template instead of a brand
- Eyebrow labels (: "MARCH SNAPSHOT" uppercase with letter-spacing)
- Hero sections inside dashboards ( has full hero-strip with decorative copy)
- Decorative copy like "Operational clarity without the clutter" as page headers
- Section notes and mini-notes everywhere explaining what the UI does
- Transform animations on hover (: translateX(2px) on nav links)
- Dramatic box shadows (: 0 24px 60px rgba(0,0,0,0.35))
- Status indicators with ::before pseudo-elements creating colored dots
- Muted labels with uppercase + letter-spacing ( overuses this pattern)
- Pipeline bars with gradient fills (: linear-gradient(90deg, var(--primary), #4fe0c0))
- KPI cards in a grid as the default dashboard layout ( has 3-column kpi-grid)
- "Team focus" or "Recent activity" panels with decorative internal copy
- Tables with tag badges for every status ( overuses .tag class)
- Workspace blocks in sidebar with call-to-action buttons
- Brand marks with gradient backgrounds (: linear-gradient(135deg, #2a2a2a, #171717))
- Nav badges showing counts or "Live" status ( has nav-badge class)
- Quota/usage panels with progress bars ( has three quota sections)
- Footer lines with meta information (: "Northstar dashboard • dark mode • single-file HTML")
- Trend indicators with colored text (: trend-up, trend-flat classes)
- Rail panels on the right side with "Today" schedule ( has full right rail)
- Multiple nested panel types (panel, panel-2, rail-panel, table-panel)



## Rule

If a UI choice feels like a default AI UI move, ban it and pick the harder, cleaner option.
- Colors should stay calm, not fight.




Dark Colorschemes
Midnight Canvas

Background: #0a0e27
Surface: #151b3d
Primary: #6c8eff
Secondary: #a78bfa
Accent: #f472b6
Text: #e2e8f0
Obsidian Depth

Background: #0f0f0f
Surface: #1a1a1a
Primary: #00d4aa
Secondary: #00a3cc
Accent: #ff6b9d
Text: #f5f5f5
Slate Noir

Background: #0f172a
Surface: #1e293b
Primary: #38bdf8
Secondary: #818cf8
Accent: #fb923c
Text: #f1f5f9
Carbon Elegance

Background: #121212
Surface: #1e1e1e
Primary: #bb86fc
Secondary: #03dac6
Accent: #cf6679
Text: #e1e1e1
Deep Ocean

Background: #001e3c
Surface: #0a2744
Primary: #4fc3f7
Secondary: #29b6f6
Accent: #ffa726
Text: #eceff1
Charcoal Studio

Background: #1c1c1e
Surface: #2c2c2e
Primary: #0a84ff
Secondary: #5e5ce6
Accent: #ff375f
Text: #f2f2f7
Graphite Pro

Background: #18181b
Surface: #27272a
Primary: #a855f7
Secondary: #ec4899
Accent: #14b8a6
Text: #fafafa
Void Space

Background: #0d1117
Surface: #161b22
Primary: #58a6ff
Secondary: #79c0ff
Accent: #f78166
Text: #c9d1d9
Twilight Mist

Background: #1a1625
Surface: #2d2438
Primary: #9d7cd8
Secondary: #7aa2f7
Accent: #ff9e64
Text: #dcd7e8
Onyx Matrix

Background: #0e0e10
Surface: #1c1c21
Primary: #00ff9f
Secondary: #00e0ff
Accent: #ff0080
Text: #f0f0f0
Light Colorschemes
Cloud Canvas

Background: #fafafa
Surface: #ffffff
Primary: #2563eb
Secondary: #7c3aed
Accent: #dc2626
Text: #0f172a
Pearl Minimal

Background: #f8f9fa
Surface: #ffffff
Primary: #0066cc
Secondary: #6610f2
Accent: #ff6b35
Text: #212529
Ivory Studio

Background: #f5f5f4
Surface: #fafaf9
Primary: #0891b2
Secondary: #06b6d4
Accent: #f59e0b
Text: #1c1917
Linen Soft

Background: #fef7f0
Surface: #fffbf5
Primary: #d97706
Secondary: #ea580c
Accent: #0284c7
Text: #292524
Porcelain Clean

Background: #f9fafb
Surface: #ffffff
Primary: #4f46e5
Secondary: #8b5cf6
Accent: #ec4899
Text: #111827
Cream Elegance

Background: #fefce8
Surface: #fefce8
Primary: #65a30d
Secondary: #84cc16
Accent: #f97316
Text: #365314
Arctic Breeze

Background: #f0f9ff
Surface: #f8fafc
Primary: #0284c7
Secondary: #0ea5e9
Accent: #f43f5e
Text: #0c4a6e
Alabaster Pure

Background: #fcfcfc
Surface: #ffffff
Primary: #1d4ed8
Secondary: #2563eb
Accent: #dc2626
Text: #1e293b
Sand Warm

Background: #faf8f5
Surface: #ffffff
Primary: #b45309
Secondary: #d97706
Accent: #059669
Text: #451a03
Frost Bright

Background: #f1f5f9
Surface: #f8fafc
Primary: #0f766e
Secondary: #14b8a6
Accent: #e11d48
Text: #0f172a
