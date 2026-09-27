# Cosmetics Hub Web

Frontend React do Cosmetics Hub, mantido separadamente da API FastAPI.

## Requisitos

- Node.js 22
- pnpm 9

## Desenvolvimento

```bash
pnpm install
pnpm dev
```

Configure `VITE_API_URL` para apontar para a API local. No estado atual, o frontend é apenas um scaffold e ainda não consome endpoints comerciais.

## Documentação comum

A documentação do produto, domínio, regras, requisitos e arquitetura está no repositório [cosmetics-hub-api](https://github.com/lc-curto/cosmetics-hub-api), em [`docs/`](https://github.com/lc-curto/cosmetics-hub-api/tree/main/docs). O contrato HTTP é a fronteira entre os repositórios.

## Validação

```bash
pnpm build
```
