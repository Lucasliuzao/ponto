# Ponto

Calculadora de horário de saída baseada nos horários de entrada e intervalos do dia. App estático (HTML + CSS + JS, sem backend), feito para uso pessoal e instalável como PWA.

🔗 **Acesse:** https://lucasliuzao.github.io/ponto/

## Funcionalidades

- Cálculo automático do horário de saída a partir da entrada e dos intervalos (almoço + um segundo intervalo opcional).
- Jornada diária configurável, com presets rápidos (8h, 8h24, 8h48, 9h) ou valor customizado.
- Indicação de horas extras quando a jornada já foi cumprida antes do horário previsto.
- Lembrete de saída: notificação do navegador com som, disparada automaticamente no horário calculado (requer permissão de notificações e a aba/app aberto).
- Horários e preferências salvos no `localStorage` do navegador — não há envio de dados para nenhum servidor.
- Instalável como PWA (ícone, splash e `manifest.json`) para uso como app na tela inicial do celular.

## Como usar localmente

Como é um site estático, basta servir a pasta com qualquer servidor HTTP simples:

```bash
python3 -m http.server 8080
```

Depois abra `http://localhost:8080/` no navegador.

## Deploy

O app é publicado via **GitHub Pages**, a partir da branch `main` deste repositório.

## Estrutura

```
index.html       # app inteiro (HTML + CSS + JS)
manifest.json     # manifest da PWA
icons/            # ícones usados pelo manifest e pelo apple-touch-icon
```
