# ZOMBIE CITY LIVE ASSETS

External runtime asset host for the Bolt/StackBlitz version of ZOMBIE CITY LIVE.

The game is configured to load Phase 4 city assets from:

https://cdn.jsdelivr.net/gh/toofe2/ZOMBIE-CITY-LIVE-ASSETS@main/assets/

Why external hosting:
- keeps binary GLB files out of the Bolt project
- avoids StackBlitz project-save PATCH 422 failures
- preserves the existing gameplay code and CommentSpawnQueue architecture

Asset folders:
- assets/city/industrial/
- assets/city/suburban/

The game includes graceful fallback behavior: a failed noncritical city asset should be skipped instead of blocking the entire Babylon scene.
