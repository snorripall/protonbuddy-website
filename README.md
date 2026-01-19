# Proton Buddy Website

[![Deploy with Coolify](https://img.shields.io/badge/Deploy%20with-Coolify-6b16ed)](https://coolify.io)

This is the website for Proton Buddy, a Linux gaming optimization tool that automatically optimizes your games for maximum performance.

## Features

- 🎮 **Automatic Game Optimization** - Detect and apply optimal launch parameters
- 📊 **Performance Tracking** - Monitor improvements across kernel updates and driver changes
- 🐧 **Universal Linux Support** - Works with Steam games, native Linux games, and any application
- ⚙️ **Flexible Configuration** - Customize DirectX to Vulkan conversions and shader pre-caching

## Tech Stack

- **Framework**: Nuxt.js 4
- **UI**: Nuxt UI (Tailwind CSS + Headless UI)
- **Icons**: Lucide + Simple Icons
- **Deployment**: Coolify (with Nixpacks)
- **Node.js**: 24 LTS

## Development

### Prerequisites

- Node.js 24+
- pnpm (recommended) or npm

### Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd protonbuddy-website
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   # or
   npm install
   ```

3. **Start development server**
   ```bash
   pnpm dev
   # or
   npm run dev
   ```

4. **Open** [http://localhost:3000](http://localhost:3000)

### Available Scripts

- `pnpm dev` - Start development server
- `pnpm build` - Build for production
- `pnpm preview` - Preview production build
- `pnpm lint` - Run ESLint
- `pnpm typecheck` - Run TypeScript type checking

## Environment Variables

### Required Environment Variables

For production deployment, set these environment variables in your deployment platform (Coolify, Vercel, etc.):

| Variable | Description | Example |
|----------|-------------|---------|
| `NUXT_PUBLIC_SITE_URL` | Full URL of your deployed site (used for SEO meta tags) | `https://protonbuddy.fourfourth.com` |

### Local Development

Create a `.env` file in the root directory:

```bash
# .env
NUXT_PUBLIC_SITE_URL=http://localhost:3000
```

**Note**: The `.env` file is ignored by Git for security. Use `.env.example` as a template.

## Deployment

### Coolify (Recommended)

1. **Connect Repository**: Add this repo to your Coolify instance
2. **Auto-Detection**: Coolify automatically detects Nuxt.js and uses Nixpacks
3. **Environment Variables**: Set `NUXT_PUBLIC_SITE_URL` in Coolify's environment variables
4. **Domain**: Configure your domain (e.g., `protonbuddy.fourfourth.com`)
5. **Deploy**: Coolify handles SSL certificates and deployment automatically

### Other Platforms

This project works with any platform that supports Nuxt.js:

- **Vercel**: Connect repo, set environment variables
- **Netlify**: Connect repo, set build command to `npm run build`
- **Railway**: Auto-detects Nuxt.js
- **Docker**: Use included `Dockerfile` and `docker-compose.yml`

## Project Structure

```
protonbuddy-website/
├── app/
│   ├── app.vue          # Main app component
│   ├── app.config.ts    # Nuxt UI configuration
│   └── pages/
│       └── index.vue    # Homepage
├── assets/
│   └── css/
│       └── main.css     # Global styles
├── public/              # Static assets
├── .env.example         # Environment variables template
├── docker-compose.yml   # Docker Compose configuration
├── Dockerfile          # Docker build configuration
├── nuxt.config.ts      # Nuxt configuration
└── package.json        # Dependencies and scripts
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally
5. Submit a pull request

## License

© 2026 Proton Buddy. Built for Linux gamers.
