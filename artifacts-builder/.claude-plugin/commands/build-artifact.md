# Build Artifact

Build and render a visual artifact (HTML, SVG, React component, or chart) based on a description or specification.

## Usage

```
/build-artifact <description>
```

## Arguments

- `description` (required): What you want to build. Can be a natural language description, a spec, or paste existing code to enhance.

## Examples

```
/build-artifact a responsive pricing table with 3 tiers: free, pro, and enterprise
```

```
/build-artifact an animated SVG loading spinner with a gradient effect
```

```
/build-artifact a bar chart showing monthly sales data for 2024
```

```
/build-artifact a React todo list component with add, complete, and delete functionality
```

## Behavior

When this command is invoked, you should:

1. **Analyze the request** to determine the best artifact type:
   - `text/html` — for full HTML pages, UI components, interactive demos
   - `image/svg+xml` — for icons, diagrams, illustrations, logos
   - `application/react` — for React components with state/interactivity
   - `application/vnd.ant.mermaid` — for flowcharts, sequence diagrams, ERDs

2. **Generate production-quality code** with:
   - Clean, semantic markup
   - Responsive design where applicable
   - Accessible attributes (aria labels, roles, alt text)
   - No external dependencies unless explicitly requested
   - Inline styles or Tailwind CSS classes for styling

3. **Render the artifact** immediately so the user can see it.

4. **Offer refinements** after rendering — ask if they want to adjust colors, layout, content, or add interactivity.

## Quality Standards

- All HTML artifacts must be valid, self-contained documents
- SVGs must have proper viewBox and be scalable
- React components must be functional components using hooks
- Charts should use clean, readable color palettes with proper labels
- Code should be commented where logic is non-obvious

## Notes

- If the description is ambiguous, make reasonable assumptions and note them
- For complex UIs, build a clean MVP first, then offer to add features
- Always prefer simplicity and clarity over complexity
