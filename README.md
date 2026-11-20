# ClassRadar 📡

Institutional Academic Copilot, Timetable Radar, and Real-Time Smart Attendance Platform for NIE North Campus.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fshaikzayanahmed%2FClass_Radar_Minor_Project&root-directory=frontend&project-name=class-radar&env=NVIDIA_API_KEY,NEXT_PUBLIC_API_URL,NEXT_PUBLIC_SOCKET_URL,NEXT_PUBLIC_NVIDIA_MODEL&envDescription=Enter%20your%20NVIDIA%20NIM%20API%20Key%20and%20Backend%20URLs&envLink=https%3A%2F%2Fbuild.nvidia.com)
[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/shaikzayanahmed/Class_Radar_Minor_Project)

---

## 🚀 One-Click Deployments

### 1. Frontend on Vercel
Click the **Deploy with Vercel** button above. Vercel will automatically configure the `frontend` Next.js application and prompt you for:
- `NVIDIA_API_KEY`: Your NVIDIA NIM key (e.g. `nvapi-...` from [build.nvidia.com](https://build.nvidia.com))
- `NEXT_PUBLIC_API_URL`: Your Fastify API URL (e.g. `https://your-api.onrender.com/api/v1`)
- `NEXT_PUBLIC_SOCKET_URL`: Your Fastify WebSocket URL (e.g. `https://your-api.onrender.com`)
- `NEXT_PUBLIC_NVIDIA_MODEL`: `nvidia/nemotron-3.5-lightning-30b-a3b`

### 2. Backend & Database on Render
Click the **Deploy to Render** button above or use **New + Blueprint** in Render:
- Provisions PostgreSQL (`classradar-postgres`)
- Deploys Fastify API & Socket.IO (`classradar-api`)
- Runs migrations (`pnpm prisma:migrate:deploy`)
- Optionally hosts the Next.js web app (`classradar-web`)
