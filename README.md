<h1 align="center">🌐 Sapper with TypeScript and Tailwindcss project base</h1>

## ❓ What is this?

This is a stripped down version of the [Sapper Typescript-GraphQL-Tailwindcss template](https://github.com/mscofield0/sapper-typescript-graphql-tailwindcss-template).

If you're looking for something with much, much more bundled in, check out [Jacob Babich's opinionated project base](https://github.com/babichjacob/sapper-firebase-typescript-graphql-tailwindcss-actions-template).

- [Sapper for Svelte](https://sapper.svelte.dev/)
  - [Official VS Code Plugin](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode)
- [PostCSS](https://postcss.org/)
  - [Tailwind CSS](https://tailwindcss.com/)
    - [Official VS Code Extension](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
      - [postcss-import](https://github.com/postcss/postcss-import)
      - [PurgeCSS](https://www.purgecss.com/)
      - [CSSNano](https://cssnano.co/)
      Inside Svelte components, thanks to [`svelte-preprocess`](https://github.com/kaisermann/svelte-preprocess)
- [TypeScript](https://www.typescriptlang.org/)
  - Inside Svelte components, thanks to [`svelte-preprocess`](https://github.com/kaisermann/svelte-preprocess)

## 📋 Copy

Choose either to clone or fork depending on your preference.

### 🐑 Clone

```sh
git clone https://github.com/mscofield0/sapper-typescript-tailwindcss-template
```

### 🍴 Fork

Click the `Use this template` button on [this project's GitHub page](https://github.com/mscofield0/sapper-typescript-tailwindcss-template).

### ⬇️ Install Dependencies

```sh
cd sapper-typescript-tailwindcss-template
npm install  # pnpm also works
```

## 🛠 Usage

### 🧪 Development
```sh
npm run dev
```

### 🔨 Building for Production
```sh
npm run prod
```

### 📦 Exporting a Static Site
```sh
npm run export
```

## ⚙ Configuration

### ⚡ Web app
Many of the fields in `static/manifest.json` (`short_name`, `name`, `description`, `categories`, `theme_color`, and `background_color`) are filled with demonstrative values that won't match your site. Similarly, you've got to take new screenshots to replace the included `static/screenshot-1.png` and `static/screenshot-2.png` files. If you want, you can add [app shortcut definitions for "add to home screen" on Android](https://web.dev/app-shortcuts/#define-app-shortcuts-in-the-web-app-manifest). Once you change `theme_color`, update the `meta name="theme-color"` tag in `src/template.html` to match.

The [Apple touch icon](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html), favicon, and `logo-` files (also all in the `static` directory) are created by placing the logo within a "safe area" centered circle that takes up 80% of the canvas's dimension. For instance, the constraining circle in `logo-512.png` is 512 × 0.80 = 409.6 ≈ 410 pixels wide and tall. 

### 🗺 Source maps
This project base comes with [source maps](https://blog.teamtreehouse.com/introduction-source-maps) enabled during development and disabled during production for the best compromise between performance and developer experience. You can change this behavior through the `sourcemap` variable in `rollup.config.js`.

## 😵 Help! I have a question

[Create an issue](https://github.com/mscofield0/sapper-typescript-graphql-tailwindcss-template/issues/new) and I'll try to help.

## 😡 Fix! There is something that needs improvement

[Create an issue](https://github.com/mscofield0/sapper-typescript-tailwindcss-template/issues/new) or [pull request](https://github.com/mscofield0/sapper-typescript-tailwindcss-template/pulls) and I'll try to fix.

I'm sorry, because of my skill level and the fragility of (the combination of) some of these tools, there are likely to be problems in this project. Thank you for bringing them to my attention or fixing them for me.

## Note on Typescript usage inside Svelte <script> tags

To use Typescript inside Svelte <script> tags, write it like so:
```sveltehtml
<script lang="ts">
    let example: string
</script>
```

## 📄 License

MIT
