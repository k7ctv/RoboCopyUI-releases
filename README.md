# RoboCopyUI &mdash; Releases

Public downloads for **RoboCopyUI**, a Windows (Delphi 12 / VCL) front-end for
`robocopy`:

- Prepare copy jobs (source, destination, options) with a live command preview
- Run jobs **detached** &mdash; reconnect and monitor status after closing the app
- Live log view; run several jobs at once
- **Live throughput** &mdash; per-job transfer rate (like Task Manager), shown as a
  single **network** figure when copying to/from a server, so you can see a running
  copy is still moving and not stalled
- **Owner logging** (optional, per job) &mdash; after a copy, append each copied
  file's NTFS owner on the source and destination to the log
- **Files-in-Browse** &mdash; the Browse dialog shows the folder's files while you
  choose it
- **Continuous log** &mdash; the log is kept across stop/edit/restart (each run
  separated), with Save-Log-As and Clear-Log
- **Orphan-proof** &mdash; the app always tracks and can stop a job's processes, plus
  a right-click *Kill Stray Processes* escape hatch
- **Watch mode** &mdash; keep a job watching the source and re-copying changes
  continuously (`/MON` after N changes, `/MOT` on a timer); shows *Watching* until
  you press Stop. Note: robocopy monitoring is a poll (it re-scans the whole source
  each cycle), not an instant trigger &mdash; frequent polling of a large tree over a
  network can be heavy

## Download

Grab the latest signed installer from the [**Releases**](../../releases) page and run it.
Installers are Authenticode-signed by *K7CTV Software*.

_(Source code is maintained in a separate private repository.)_