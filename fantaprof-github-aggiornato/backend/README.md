# Backend Fantaprof

Deploy Node.js 20+: `npm install`, start `npm start`. Configure `JWT_SECRET` as a random secret of at least 32 characters. Configure `DATA_FILE` on persistent disk (e.g. `/var/data/fantaprof.json`) so user data survives redeploys. Use HTTPS.

Endpoints for invitations: POST `/api/leagues` with `{name,state}` returns a code; POST `/api/leagues/join` with `{code}` joins an account; GET `/api/leagues` lists memberships.

IMPORTANT: the current frontend still uses the personal `/api/state` backup. The invite endpoints are available, but full shared gameplay requires wiring the game to `/api/leagues/:id/state`; this ZIP is not yet a verified end-to-end multiplayer release. Test two accounts before inviting players.
