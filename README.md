# Clima Agora 🌤️

App simples: **backend Node** (sem dependências) que consome a API pública [Open-Meteo](https://open-meteo.com) + **frontend** para visualizar o clima atual de uma cidade.

## Como rodar

Requer Node 18 ou superior.

```bash
cd clima-app
npm start
```

Depois abra no navegador: http://localhost:3000

## Como funciona

- `server.js` — servidor HTTP. Serve os arquivos da pasta `public/` e expõe o endpoint `/api/clima?cidade=NOME`, que busca a cidade no Open-Meteo (geolocalização + clima atual).
- `public/` — frontend (HTML, CSS e JS) que consome o endpoint e mostra temperatura, condição e vento.

## Estrutura

```
clima-app/
├── server.js          # backend
├── package.json
└── public/
    ├── index.html     # interface
    ├── style.css      # estilos
    └── app.js         # lógica do frontend
```
