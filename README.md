# Tailwind CSS + Vite Setup 🚀

## 1️⃣ Install
```bash
npm install tailwindcss @tailwindcss/vite

2️⃣ Configure Vite (vite.config.js)
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [tailwindcss()],
})

3️⃣ Import Tailwind (src/index.css)
@import "tailwindcss";

4️⃣ Run Dev
npm run dev

