# ALVOS 🎯

**ALVOS** é um painel pessoal offline-first para transformar objetivos em ações e acompanhar progresso — pensado para telemóvel e para funcionar sem API paga, base de dados ou internet.

## Funcionalidades atuais

- Dashboard **Hoje** com foco diário e checklist.
- Temporizador de foco de 25 minutos.
- Metas financeiras em Kz, incluindo progresso para 80.000 Kz/mês.
- Área de **Estudos — Enfermagem** com disciplinas prioritárias e tarefas.
- Registo de entradas, saídas e saldo.
- Calculadora de importação/revenda: custo real, lucro, margem e markup.
- Calculadora de lucro, margem e markup.
- Calculadora de meta diária.
- Gestão de projetos com progresso e estado.
- Notas rápidas.
- Backup **exportar/importar JSON**.
- Persistência local no dispositivo.
- Interface responsiva e mobile-first.
- Escapamento de texto inserido pelo utilizador para reduzir problemas de HTML injetado.
- Compatibilidade/migração de dados das versões anteriores `alvos-v2` e `meu_rumo_pro_v2`.
- Datas das tarefas calculadas no fuso horário local do dispositivo, evitando o erro de virar o dia por causa de UTC.

## Como usar

Abra o `index.html` no navegador. Os dados são guardados localmente no dispositivo.

**Importante:** como os dados ficam no navegador, exporta um backup JSON periodicamente, sobretudo antes de limpar os dados do navegador ou trocar de telemóvel.

## Publicar no GitHub Pages

No GitHub: **Settings → Pages → Deploy from a branch → main → /(root)**.

Depois, abre o endereço do GitHub Pages no telemóvel e adiciona-o ao ecrã inicial, se o navegador oferecer essa opção.

## Próximas evoluções

1. PWA instalável com manifesto e Service Worker.
2. Calendário e prazos para metas/tarefas.
3. Gráficos de evolução.
4. Hábitos e sequência de dias.
5. Modo estudo com histórico de sessões.
6. Notificações locais.
7. Melhorias de acessibilidade e navegação por teclado.
8. Sincronização opcional com Supabase.

> O projeto mantém uma abordagem local-first: as funções essenciais devem continuar utilizáveis sem serviços pagos.
