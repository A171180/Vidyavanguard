# Dibba Bolega exact prototype recreation

## Goal
Rebuild the supplied reference as a mobile-first, single-page React prototype using mock data only, preserving its layout, colors, typography, animated bin characters, wording, roles, and workflows.

## Build
- Recreate the Hindi-first login screen exactly, including language selector, role/user selection, animated bin showcase, and responsive desktop/mobile composition.
- Build the shared signed-in shell with the same header, language controls, voice guide, role identity, navigation, footer, and reset behavior.
- Implement Villager screens: pickup request, segregation guide, and post-pickup driver rating with required reason, photo, and playable voice-note recording.
- Implement Driver screens: full/requested-bin route, route savings, collection and waste weights, sensor-weight warning, and household rating.
- Implement GP screens: overview/map and live bin sliders, driver scorecard, stock/income and enquiry decisions, and complaints with voice playback.
- Implement Buyer screens: buyer selection, stock-demand comparison, enquiries, and the high-demand insight.
- Keep all state shared in the browser so the required cross-role demo flows work without a backend.

## Technical details
- Use the existing TanStack Start app and Tailwind v4 token system.
- Keep one content route at `/`; role views remain in-app screens.
- Use Lucide icons and CSS-built animated bin characters matching the reference.
- Use browser speech synthesis and MediaRecorder where supported; show the specified Punjabi-audio fallback.
- Add route-specific social metadata, a short README, and focused interaction tests.
- Verify the reference-matched login plus all four roles on mobile and desktop, then check current build diagnostics.
