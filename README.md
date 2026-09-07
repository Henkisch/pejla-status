# pejla-status

Pejla's public status page — [status.pejla.app](https://status.pejla.app).

Runs on [Upptime](https://github.com/upptime/upptime): GitHub Actions pings
each service every 5 minutes and commits the result to this repo; GitHub
Pages serves the static status site built from that history. Deliberately
independent of Vercel/our own infrastructure so the status page stays
reachable even if Pejla itself is down.

Monitors: the marketing site and app (pejla.app / my.pejla.app), plus the
official status pages of every third-party service Pejla depends on
(Vercel, Neon, Clerk, Resend, Sanity) and a direct ping of Skatteverket's
API host (no public Skatteverket status page exists).

Config lives in [`.upptimerc.yml`](.upptimerc.yml). To add or change a
monitored site, edit that file and push — no other setup needed.
