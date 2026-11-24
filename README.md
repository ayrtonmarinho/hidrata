# Hidrata — lembrete de beber água

App Android offline que calcula a meta diária de água pelo peso (35 ml/kg, ajustável), divide entre o horário
de acordar e o de dormir e lembra a cada dose com notificação. Dias de treino somam um extra na meta.
As doses que faltam são recalculadas conforme você bebe, e lembretes de doses que você já bebeu adiantado são pulados.

## Como gerar o APK
Todo `push` na `main` dispara o GitHub Actions (`.github/workflows/build-apk.yml`), que compila e publica em **Releases**.

## Instalar
Baixe o `Hidrata-vN.apk` em Releases pelo celular e abra. Para atualizar, instale a versão nova por cima.

## Estrutura
- `www/index.html` — o app (um arquivo só)
- `android/` — projeto Android gerado pelo Capacitor 7
- `android/app/hidrata.keystore` — chave de assinatura fixa (mantenha o repositório **privado**)
