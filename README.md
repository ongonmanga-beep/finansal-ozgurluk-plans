# Finansal Özgürlük Projesi - Plan ve Dokümantasyon

## Proje Özeti

Portföy takibi ve finansal özgürlük hedeflerini yönetmek için **Svelte + SvelteKit** web uygulaması.

## Teknoloji Stack

- **Frontend:** SvelteKit 2.0 + TypeScript + Tailwind CSS
- **Database:** PostgreSQL (Supabase) - Remote
- **Auth:** Supabase Auth (Email/Password)
- **Real-time:** Supabase Realtime subscriptions
- **Charts:** LayerChart + D3.js
- **Deployment:** VPS (IP-only initially)

## Deployment Strategy

**Workflow: Lokal Development → VPS Deployment**

- Lokal development (localhost)
- Production build test (lokal)
- VPS transfer (SCP/rsync)
- Self-hosted with PM2 + Nginx
- IP-only deployment (domain optional)

## Cost

- **VPS:** €3.5-6/month (Hetzner/DigitalOcean)
- **Supabase:** Free tier (500MB storage)
- **Domain:** €10-15/year (optional)
- **Total:** €42-72/year

## Timeline

- **Faz 1:** Setup (1 week)
- **Faz 2:** Auth (1 week)
- **Faz 3:** Portfolio CRUD (2-3 weeks)
- **Faz 4:** Market Data (2-3 weeks)
- **Faz 5:** Goals (1-2 weeks)
- **Faz 6:** Budget (1-2 weeks)
- **Faz 7:** Reports + PWA (1-2 weeks)
- **Faz 8:** Testing + VPS Deploy (1 week)
- **Total:** 9-13 weeks

## Dokümantasyon

- `PLAN.md` - Detaylı uygulama planı
- `MEMORY.md` - Proje hafızası ve kararlar

## Başlangıç

```bash
# SvelteKit proje oluştur
npm create svelte@latest finansal-ozgurluk

# Supabase setup
supabase projects create finansal-ozgurluk --region eu-west-1
```

## İletişim

Proje sahibi: @hayli