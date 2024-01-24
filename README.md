# Next.js Snippets for VS Code

This extension provides useful code snippets for developing Next.js applications in Visual Studio Code.

## Features

### Available Snippets

-   `npg` or `newpage`,: Creates a new NextJS page.tsx.
-   `nly` or `newlayout`,: Creates a new NextJS layout.tsx.

## Usage

1. Install the "Next.js Snippets" extension in Visual Studio Code.
2. Open a Next.js file.
3. Type the desired snippet shortcut and press `Tab` to insert the code.

## Snippets

### `npg` or `newpage` - Creates a new NextJS page.tsx

Example:

```tsx
'use client';

interface HeroProps {}

const Hero = ({}: HeroProps) => {
    return (
        <div>
            <h1>Hero</h1>
        </div>
    );
};

export default Hero;
```

### `nly` or `newlayout` - Creates a new NextJS layout.tsx

Example:

```tsx
// Import your globals here
// import "@/styles/globals.css";

import { Inter } from 'next/font/google';

const inter = Inter({
    subsets: ['latin'],
});

export const metadata = {
    title: 'New page title here',
    description: 'Sample description',
};

export default function RootLayout({ children }: { children: React.ReactNode }) {
    return (
        <html lang="en">
            <body className={inter.className}>{children}</body>
        </html>
    );
}
```

## License

This extension is licensed under the MIT License.
