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

Use o Expo Go no celular para escanear o QR code ou execute no emulador:
- Android: `npm run android`
- iOS: `npm run ios`

## Contas de demonstração

Senha para todas: `123456`

- **Médico:** joao@example.com, maria@example.com
- **Paciente:** teste@paciente.com, ana@exemplo.com
