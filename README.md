# ALVOS — Centro de Execução

ALVOS é um painel pessoal **mobile-first, offline-first e sem API paga** para transformar objetivos em execução.

## O que mudou na v4

- **Hoje:** foco do dia, tarefas, prioridades, hábitos e revisão diária.
- **Planeamento:** pesquisa e filtros por hoje, próximos 7 dias e atrasadas.
- **Tarefas detalhadas:** data, prioridade e categoria.
- **Estudos:** mapa das disciplinas, tarefas de estudo e indicadores semanais.
- **Deep Focus:** 25/50 minutos, pausa, reset e recuperação do timer após recarregar a página.
- **Hábitos:** marcação diária e sequência (streak).
- **Dinheiro:** entradas, saídas, saldo e meta de 80.000 Kz/mês.
- **Importação/revenda:** custo real, lucro, margem e markup.
- **Projetos:** progresso, estado e próximo passo.
- **Insights:** leitura simples dos últimos 7 dias, alertas e histórico de foco.
- **Notas e revisão diária:** conhecimento e decisões ficam no mesmo lugar.
- **Backup JSON:** exportação e restauração.
- **PWA:** manifesto, ícone e service worker para cache/offline.
- **Persistência local:** dados guardados no dispositivo.
- **Migração:** versões anteriores (alvos-v3, alvos-v2 e meu_rumo_pro_v2) são lidas e normalizadas.
- **Data local:** datas são calculadas no relógio local do dispositivo, evitando o erro de UTC perto da meia-noite.
- **Segurança de interface:** conteúdo introduzido pelo utilizador é escapado antes de entrar no HTML.

## Princípios de produto usados

A arquitetura da v4 incorpora padrões recorrentes em aplicações de produtividade: captura rápida, vista “Hoje”, prioridades, filtros, decomposição de tarefas, projetos com progresso, hábitos/streaks, foco temporizado, revisão e métricas. O objetivo foi trazer esses padrões sem transformar o ALVOS num sistema pesado.

## Privacidade e limitações

O ALVOS não envia os teus dados para um servidor. Isso melhora a simplicidade e o funcionamento offline, mas significa que **a perda do armazenamento do navegador pode causar perda de dados**. Exporta backups regularmente.

O service worker melhora o acesso offline depois da primeira carga em ambiente HTTPS/GitHub Pages. Ele não substitui o backup.

## GitHub Pages

1. Abra **Settings → Pages** no repositório.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Escolha `main` e a pasta `/root`.
4. Guarde e abra o endereço Pages disponibilizado pelo GitHub.

## Estrutura

- `index.html` — aplicação e lógica principal.
- `manifest.webmanifest` — instalação como PWA.
- `sw.js` — cache/offline.
- `icon.svg` — ícone da aplicação.

## Roadmap

- calendário visual e arrastar/reordenar;
- tarefas recorrentes;
- notificações locais quando suportadas pelo navegador;
- gráficos mais completos;
- exportação CSV;
- sincronização opcional com Supabase;
- testes automatizados mais extensos.

**Versão atual: 4.0**
