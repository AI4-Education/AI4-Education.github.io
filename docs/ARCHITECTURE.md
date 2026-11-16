# Growth architecture

The public information layer uses semantic standalone HTML, shared design tokens and isolated browser interactions. It can remain the public site while application services are introduced incrementally. This foundation supports extension; accounts and AI services still require new implementation.

## Suggested boundaries

- Public content: retain existing six URLs and navigation.
- Resources: add curriculum and subject metadata when real materials exist; move repeated content to a CMS or build-time data layer as its volume grows.
- Learning workspace: add under `app/` or a separate application origin while retaining branding and public routes.
- Services: integrate through a versioned HTTPS API, for example `/api/v1/`, with server-side authentication, validation, rate limits and audit logs.
- AI: keep model credentials and prompt orchestration on the server. Never put secret API keys in HTML, browser JavaScript or a GitHub repository. GitHub Pages provides static hosting only; use a separate backend or migrate application hosting.
- Identity: use a mature authentication provider. Enforce authorization on the server, including teacher/student roles and school tenancy if required.
- Data: introduce consent, retention and deletion rules before collecting student information. Use minimal data, clear purpose and explicit access controls.

## Delivery sequence

1. Publish approved content and accessible classroom resources.
2. Validate one pilot tool with educators. Add backend services, monitoring and safety review for that tool.
3. Introduce optional accounts and learner progress only when an evaluated need justifies their data collection.
4. Add curriculum-aligned pathways and integrations without replacing the public information site.

## Accessibility and quality

Maintain keyboard navigation, visible focus, semantic headings, readable contrast and reduced-motion support. Before release, check mobile menus, project filters, form validation, screen-reader labels and layout at phone, tablet and desktop widths. Test real services independently when added; browser-only demonstrations should remain explicitly labelled.
