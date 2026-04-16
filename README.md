# @notevome/notevo-shadcn-theme

A custom, reusable **shadcn/ui** theme for Notevo projects.

Includes clean light & dark mode, sidebar styles, novel/editor variables, and more.

## Installation

```bash
npm install @notevome/notevo-shadcn-theme

pnpm add @notevome/notevo-shadcn-theme

```

## Usage
In your main CSS file (app/globals.css or src/index.css):
 ```ts
@import "tailwindcss";
@import "@notevome/notevo-shadcn-theme";
```
Make sure your components.json has CSS variables enabled:
```json
{
  "tailwind": {
    "cssVariables": true
  }
}
```
## Dark Mode
Add dark class to your <html> tag:
```html
<html lang="en" class="dark">
```

## Force Light Mode
Use this class anywhere to force light mode:
```html
<div class="force-light">
  ...
</div>
```

## Example
Add all shadcn components (Button, Card, Input, etc.) will automatically use your custom colors.
```ts
import { Button } from "@/components/ui/button";

export default function Page() {
  return <Button>Primary Button – Uses Notevo Theme</Button>;
}
```
## Development

```bash
# Clone repo
git clone https://github.com/notevome/notevo-shadcn-theme.git
cd notevo-shadcn-theme

# Install dependencies (optional, for testing)
npm install

# Publish new version
npm version patch          # or minor / major
npm publish --access public
```
# License
MIT © Notevo
