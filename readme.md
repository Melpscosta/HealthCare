# HealthConnect - Marcação de Consultas Médicas

Aplicativo mobile para agendamento de consultas médicas, desenvolvido com React Native e Expo.

## Sobre

O HealthConnect permite que pacientes agendem consultas com médicos de forma simples. Os médicos podem aceitar solicitações, ver observações dos pacientes e trocar mensagens após a confirmação.

## Funcionalidades

### Paciente
- Login e cadastro
- Agendar consultas (médico, data e horário conforme disponibilidade)
- Ver histórico de consultas
- Trocar mensagens com o médico após confirmação

### Médico
- Login
- Ver agenda de consultas pendentes e confirmadas
- Aceitar ou recusar consultas
- Ver observações do paciente
- Enviar mensagens ao paciente

## Tecnologias

- React Native + Expo
- TypeScript
- Styled Components
- React Navigation
- AsyncStorage

## Como executar

```bash
npm install
npm start
```

Use o Expo Go no celular para escanear o QR code ou execute:
- Android: `npm run android`
- iOS: `npm run ios`
- Web (navegador): `npm run web`

Se o terminal não reconhecer `expo` no Windows, use sempre os scripts npm do projeto (`npm start`, `npm run web`, etc.), pois eles já chamam o Expo local via `npx`.

## Publicar em link na Vercel (Expo Web)

Este projeto pode ser publicado como site estático (versão web do app).

### 1) Gerar build web

Na raiz do projeto:

```bash
npx expo export -p web
```

Esse comando gera os arquivos estáticos em `dist`.

### 2) Publicar pela Vercel (mais simples)

1. Suba o projeto para o GitHub.
2. Acesse [Vercel](https://vercel.com), clique em **Add New > Project**.
3. Importe o repositório.
4. Em configurações de build:
   - **Framework Preset:** `Other`
   - **Build Command:** `npx expo export -p web`
   - **Output Directory:** `dist`
5. Clique em **Deploy**.
6. A Vercel vai gerar um link público (ex: `https://seu-projeto.vercel.app`).

### 3) Publicar via CLI (alternativa)

```bash
npm i -g vercel
vercel login
vercel
```

Quando a CLI perguntar:
- Build command: `npx expo export -p web`
- Output directory: `dist`

Para publicar produção depois:

```bash
vercel --prod
```

### 4) SPA/rotas (opcional, mas recomendado)

Se houver navegação por URL no web app, crie `vercel.json` na raiz:

```json
{
  "rewrites": [
    { "source": "/(.*)", "destination": "/index.html" }
  ]
}
```

## Contas de demonstração

Senha para todas: `123456`

- **Médico:** joao@example.com, maria@example.com
- **Paciente:** teste@paciente.com, ana@exemplo.com
