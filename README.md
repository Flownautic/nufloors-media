# nufloors-media

Staging area for the Nufloors content engine. **Nothing here is authored.**

Instagram, Facebook and Google Business all fetch post images from a public URL
rather than accepting an upload, and the engine's own storage (a private Google
Drive) cannot serve one. So rendered frames are copied here for a few days while
the platforms fetch them, then removed.

- Files live under `media/<YYYY-MM-DD>/` and are named by a hash of their
  contents, so a path is never reused.
- They are pruned after 7 days (`npm run publish:host -- --prune`).
- Every image here is one that was about to be posted publicly anyway.

The engine itself, its briefs and its data are in a separate private repository.
