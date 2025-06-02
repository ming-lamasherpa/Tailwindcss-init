# Tailwindcss-init

1) Install Tailwind CSS
Install tailwindcss and @tailwindcss/vite via npm.
=> npm install tailwindcss @tailwindcss/vite

2) Configure the Vite plugin
Add the @tailwindcss/vite plugin to your Vite configuration.
=>
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'
export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})

3) Import Tailwind CSS
Add an @import to your CSS file that imports Tailwind CSS.
=> @import "tailwindcss";

4) Start your build process
Run your build process with npm run dev or whatever command is configured in your package.json file.
=> npm run dev

5) Start using Tailwind in your HTML
Make sure your compiled CSS is included in the <head> (your framework might handle this for you), then start using Tailwind’s utility classes to style your content.
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/src/styles.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>

Chat box :
<div class="mx-auto flex max-w-sm items-center gap-x-4 rounded-xl bg-white p-6 shadow-lg outline outline-black/5 dark:bg-slate-800 dark:shadow-none dark:-outline-offset-1 dark:outline-white/10">
  <img class="size-12 shrink-0" src="/img/logo.svg" alt="ChitChat Logo" />
  <div>
    <div class="text-xl font-medium text-black dark:text-white">ChitChat</div>
    <p class="text-gray-500 dark:text-gray-400">You have a new message!</p>
  </div>
</div>
