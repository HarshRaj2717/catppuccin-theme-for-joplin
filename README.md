<h1 align="center">
  <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
  Catppuccin for Joplin
</h1>

<h6 align="center">
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-installation">🔧 Installation</a>
  ·
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-floating-markdown-toc">🎈 Floating TOC</a>
  ·
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-additional-syntax-highlighting">🎨 Additional highlighting</a>
  ·
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#-hidden-elements">🥷 Hidden elements</a>
  ·
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#%EF%B8%8F-spoilers">⬇️ Spoilers</a>
  ·
  <a href="https://github.com/sadmice/Catppuccin-Theme-For-Joplin#%EF%B8%8F-mermaid">🧜‍♀️ Mermaid</a>
</h6>

![image](https://user-images.githubusercontent.com/23323305/168392162-44a6be18-b75d-4796-97df-559635da1fbb.png)

## 🔧 Installation

### ✍️ Install fonts

- Regular: [Fira Sans](https://fonts.google.com/specimen/Fira+Sans)
- Monospace: [Fira Code](https://github.com/tonsky/FiraCode)

### 🖼️ Install Theme

1. Open Joplin
2. Go to `Tools` > `Options` > `Appearance` > `Theme`
3. Choose `Dark`
4. Click `Apply`
5. In the same page, Click `Show Advanced Settings`
6. Click `Custom stylesheet for rendered Markdown`
7. Copy [Catppuccin userstyle.css code](https://github.com/sadmice/Catppuccin-Theme-For-Joplin/blob/main/userstyle.css)
8. Paste it on your `userstyle.css`
9. Click `Custom stylesheet for Joplin-wide app styles`
10. Copy [Catppuccin userchrome.css code](https://github.com/sadmice/Catppuccin-Theme-For-Joplin/blob/main/userchrome.css)
11. Paste it on your `userchrome.css`
12. Restart Joplin

## 💡 Tips

### 🎈 Floating Markdown TOC

![image](https://user-images.githubusercontent.com/23323305/168394747-64052ed6-295c-40d0-bd1a-a8ce06ce1421.png)

To use the table of contents, you need to:

- Enable toc in your settings
  - Go to `tools` > `Options` > `Markdown`
  - `Enable table of contents extension`
  - Click `Apply`
- Include `[[toc]]` in your markdown
- Hover your mouse over the right side of the render viewer

### 🎨 Additional syntax highlighting

To see all custom syntax highlighting, you first need to enable it in Joplin:

1. Go to `tools` > `Options` > `Markdown`
   - Enable Mermaid diagrams support
   - Enable ==mark== syntax
   - Enable footnotes
   - Enable table of contents extension
   - Enable abbreviation syntax
   - Enable ++insert++ syntax
2. Click `Apply`

Some of them require the Rich Markdown plugin to see them highlighted in the Markdown Editor

1. Go to `tools` > `Options` > `Plugins`
2. Search the plugin `Rich Markdown`
3. Click `Install`
4. Restart Joplin
5. Go to `tools` > `Options` > `Rich Markdown`
6. Enable the `Add additional CSS classes for enhanced customization`
7. Press `OK`

### 🥷 Hidden elements

Some Joplin's UI elements are hidden by default, but you can return them if you need to.

#### "All Notes" button

Change the `all-notes-button-display` variable on line 28 of userchome.css from `none` to `flex`.

```css
--all-notes-button-display: none; /* hidden */
--all-notes-button-display: flex; /* shown */
```

#### Rich Text Editor Switch

Change the `rich-text-editor-switch-button-display` variable on line 29 of userchome.css from `none` to `flex`.

```css
--rich-text-editor-switch-button-display: none; /* hidden */
--rich-text-editor-switch-button-display: flex; /* shown */
```

#### "New Todo" button

Change the `new-todo-button-display` variable on line 30 of userchome.css from `none` to `flex`.

```css
--new-todo-button-display: none; /* hidden */
--new-todo-button-display: flex; /* shown */
```

### ⬇️ Spoilers

![image](https://user-images.githubusercontent.com/23323305/168396760-f56100af-0c14-43f2-9386-d333f07e77db.png)

This theme contains styling for the Spoilers plugin.

1. Go to `tools` > `Options` > `Plugins`
2. Search the plugin `Spoilers`
3. Click `Install`
4. Restart Joplin

### 🧜‍♀️ Mermaid

![image](https://user-images.githubusercontent.com/23323305/168396949-894fcb6e-834b-49d2-ad3b-9b0c6a359a18.png)

To see your mermaid charts better, enable a dark theme for them by including `%%{init: { "theme" : "dark", "flowchart" : { "curve" : "basis" } }%%%` in your mermaid markdown.
