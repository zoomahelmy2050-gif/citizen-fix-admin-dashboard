# Upload Files to GitHub

Go to: https://github.com/zoomahelmy2050/citizen-fix-admin-dashboard

## Method 1: Drag and Drop (Easiest)
1. Click "uploading an existing file"
2. Drag ALL files from C:\citizen-fix-admin-dashboard (except .git folder)
3. Commit changes

## Method 2: Create each file manually
Copy and paste each file content:

### 1. package.json
```json
{
  "name": "citizen-fix-admin",
  "private": true,
  "version": "0.1.0",
  "scripts": {
    "dev": "next dev -p 4000",
    "build": "next build",
    "start": "next start"
  },
  "dependencies": {
    "next": "14.2.5",
    "react": "18.2.0",
    "react-dom": "18.2.0",
    "swr": "2.2.5",
    "react-leaflet": "4.2.1",
    "leaflet": "1.9.4"
  },
  "devDependencies": {
    "typescript": "5.5.4",
    "@types/node": "22.7.4",
    "@types/react": "18.2.69",
    "@types/react-dom": "18.2.22"
  }
}
```

### 2. next.config.js
```js
/** @type {import('next').NextConfig} */
const nextConfig = {
  experimental: {
    appDir: true,
  },
};

module.exports = nextConfig;
```

### 3. tsconfig.json
```json
{
  "compilerOptions": {
    "target": "ES2022",
    "lib": ["dom", "dom.iterable", "esnext"],
    "allowJs": false,
    "skipLibCheck": true,
    "strict": true,
    "noEmit": true,
    "esModuleInterop": true,
    "module": "esnext",
    "moduleResolution": "bundler",
    "resolveJsonModule": true,
    "isolatedModules": true,
    "jsx": "preserve",
    "incremental": true,
    "forceConsistentCasingInFileNames": true
  },
  "include": ["next-env.d.ts", "**/*.ts", "**/*.tsx"],
  "exclude": ["node_modules"]
}
```

Then create the app/, components/, and lib/ folders with their respective files.
