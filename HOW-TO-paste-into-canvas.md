# How to Use AI-Designed Pages in Canvas — Without Giving AI Any API Access

This workflow lets you (or anyone) design a Canvas page with AI, then upload it **manually**.
No API token, no automated access to Canvas is required. The AI only produces HTML;
a human does the uploading.

---

## Why it works

Canvas's page editor has a built-in **HTML source view**. The AI-generated designs use
only **inline styles** (`style="..."` on each tag) — no `<script>`, no `<style>` blocks,
no external fonts. These are exactly what Canvas accepts, so the HTML pastes in cleanly
and renders identically to the preview.

---

## Steps (same for editing the homepage or making a brand-new page)

1. In Canvas, open the course → **Pages** → **+ Page** (or open an existing page → **Edit**).
2. In the Rich Content Editor, click the **`</>`** button (bottom-right) to switch to **HTML view**.
3. **Select all and paste** the AI-provided HTML into that box.
4. Click **Save**.
5. (For a new homepage) On the page, click **⋮ → Use as Front Page**, then in
   **Course Settings → Choose Home Page → Pages Front Page**.

## The banner image

1. Upload your image to Canvas → **Files** first.
2. Either insert it with the editor's image button, or paste an
   `<img src="...your Canvas file link...">` tag into the HTML.
   (Canvas file links work for all enrolled students.)

---

## Division of labour

- **AI**: designs the page, outputs a single block of inline-styled HTML. Previewable in a
  browser or via a shared link before anything touches Canvas.
- **Human**: copies that HTML and pastes it into the Canvas HTML view. Full control,
  full review, nothing automated.

---

## 中文摘要

这套流程让 AI 只负责"设计 + 出 HTML"，上传由人手动完成，**全程不需要给 AI 任何 Canvas API 授权**。

原理：Canvas 页面编辑器有 `</>` HTML 源码视图，而 AI 生成的设计全部用内联样式
（不含脚本、不含外部字体），Canvas 完全接受。

步骤：课程 → Pages → 新建/编辑 → 点 `</>` → 粘贴 HTML → Save →（首页的话）
⋮ → Use as Front Page。Banner 图先传到 Files 再插入即可。
