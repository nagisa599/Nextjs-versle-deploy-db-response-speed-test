# Nextjs(Vercel) 　 ✖️ DB(Posgress(vercel) 　における応答速度調査

このリポジトリは、Nextjs(vercel)とPosgress(vercel)を利用した場合の応答速度を調べるためのリポジトリーです


[本番環境](https://nextjs-versle-deploy-db-response-speed-test.vercel.app/)


## DB Migration

```bash
# migration
pnpm run drizzle:migrate
```

## Nextjs の立ち上げ方

```bash
pnpm run dev
```

## Vercel のデプロイする時に注意すること

package.json の build をいかに変更

```json
 "build": "drizzle-kit generate && drizzle-kit migrate &&  next build",
```

