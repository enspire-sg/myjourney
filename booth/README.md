# Aquila Booth Shifts static shell

GitHub Pages candidate for `https://enspire-sg.github.io/booth/`.

The page is static. It calls the existing Apps Script deployment through the explicit `?api=1` text/plain JSON bridge. The Apps Script-hosted `Index.html` remains unchanged as rollback.

## Rollout

1. Deploy the Apps Script backend after the complete local gate is green.
2. Publish this directory as the root of the public `enspire-sg/booth` GitHub Pages repository.
3. Test the final Pages origin in a real browser: OTP, Journey fragment handoff, cached cold open, every write path, sign-out/cache clearing, and CORS redirect handling.
4. Keep the old Apps Script URL available until the team migration is verified.
