# SHADCN/UI compnents
a fan implamentation of the SHADCN/UI project as an NPM library



# installation 
```bash
 npm i shadcn-fe-components
 yarn add shadcn-fe-components
 pnpm add shadcn-fe-components
```
⚠ this project does not ship css files and assumes you're already using tailwind , the styles will be derived from the component tailwind classnames

Add this to your `tailwind.config.js`
 ```js
   content: [
  './src/app/**/*.{ts,tsx}',
    './node_modules/shadcn-fe-components/dist/**/*.{js,ts,jsx,tsx}'
      
	]
 ```
you can also be selective and only load the css for the files you've used

for everything in button styles
 ```js
   content: [
  './src/app/**/*.{ts,tsx}',
    './node_modules/shadcn-fe-components/dist/button/{*}.{js,ts,jsx,tsx}'
      
	]
 ```
 for a specific button.tsx styles
 ```js
   content: [
  './src/app/**/*.{ts,tsx}',
    './node_modules/shadcn-fe-components/dist/**/button.tsx'
      
	]
 ```
you can then import
> 
```tsx
import { Button } from "shadcn-fe-components"
```

## helpful references
[relase-it + github actions setup video](https://www.youtube.com/watch?v=7pBcuT7j_A0)
