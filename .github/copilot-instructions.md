<!-- Copilot / AI agent guidance for this repository -->
# Copilot instructions — Communicate using Markdown

Purpose: Help AI agents make small, safe, and repository-consistent edits to this GitHub Skills course repository.

Big picture
- This repository is a single-course content repo: the primary source files are [README.md](README.md) and [index.md](index.md). It contains authored Markdown (with some HTML wrapper fragments) and a license.
- There is no build system, runtime, or test suite — content is intended for direct rendering by GitHub and VS Code Markdown preview.

What to preserve
- Preserve the HTML header/footer comment blocks used in the course README (do not remove or reformat the author-note comments in the top-of-file HTML fragment in [README.md](README.md)).
- Keep the `1280×640` social image requirement and sentence-case course title when editing the header block.

Editing patterns and examples
- Follow the style in [index.md](index.md) for lesson content: short headings, fenced code blocks, images, and task lists.
- When updating the course header, maintain the structure: an HTML `<header>` element containing the title, brief description, and an author-note comment. Example pattern (preserve comments):

```html
<header>
  <!-- <<< Author notes: Course header >>> -->
  # Course Title
  _Short description._
</header>
```

Developer workflows (repo-specific)
- No build or test commands are required — preview changes locally using VS Code Markdown preview or by pushing to GitHub and enabling Pages. The README includes explicit GitHub Pages setup steps.
- For changes that affect course metadata (title/image/license), also update the `README.md` header and keep the MIT license reference intact in `LICENSE`.

Conventions and tone
- Keep language friendly and instructional — matches the course tone in [README.md](README.md).
- Use concise examples and short lesson snippets. Prefer sentence-case headings.

Integration points and external dependencies
- This repo publishes as static Markdown via GitHub; there are no external code dependencies. Links to GitHub Skills resources and external docs should remain intact.

When in doubt
- Make minimal, reversible edits. Open a draft PR with a clear title describing the course improvement. Avoid restructuring the repository or introducing build tooling.

If you need more context or specific examples, ask for which lesson or file to target.
