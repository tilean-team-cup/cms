# CMS — tilea.net

Stack CMS per tilea.net basato su Directus + PostgreSQL, deployato su LXC 103 (192.168.1.22).

## Servizi

| Servizio | Porta | Dominio pubblico |
|----------|-------|-----------------|
| Directus | 8055 | cms.tilea.net |
| PostgreSQL | 5432 | — (interno) |

## Setup

```bash
git clone https://github.com/tilean-team-cup/cms /root/cms
cd /root/cms
cp .env.example .env
# edita .env con i valori reali
docker compose up -d
```

## Comandi utili

```bash
docker compose up -d          # avvia
docker compose down           # ferma
docker compose logs -f directus  # log
docker compose pull && docker compose up -d  # aggiorna
```
