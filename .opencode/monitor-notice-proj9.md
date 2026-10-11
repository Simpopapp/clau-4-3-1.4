# Aviso pendente ao monitor (OpenCode)

- Data: 2026-10-11 (UTC, última tentativa) · Atualizado: 2026-10-11 (UTC)
- Tentativa: `curl http://127.0.0.1:4096/api/health` falhou (sem processo na porta 4096) e o
  binário `opencode` não existe no sandbox (`/root/.bun/bin/opencode` ausente).
- Mensagem a entregar quando o monitor estiver no ar: "remix finalizado (+Fase 4 do roadmap-proj9)"
- Fase 1 (integridade do progresso, storage v6) concluída com todos os gates verdes:
  vitest 266/266 · tsgo limpo · build OK · lint 0 erros · Playwright OK.
- Fase 2 (SRS correto) concluída com todos os gates verdes:
  vitest 285/285 (23 novos em `srs-v2.test.ts`) · tsgo limpo · build OK · lint 0 erros ·
  Playwright OK (fase não toca UI).
- Fase 3 (medição honesta em fala e escrita) concluída com todos os gates verdes:
  vitest 299/299 (14 novos em `fase3.test.ts`) · tsgo limpo · build OK ·
  lint 0 erros (8 warnings pré-existentes) · Playwright 390×844 OK
  (subscores Conteúdo/Fluência/Pronúncia, aviso de microfone no 1º uso,
  aviso de template no SST, console limpo).
- Fase 4 (escala, alvo e prontidão) concluída com todos os gates verdes:
  vitest 324/324 (+25: `estimate.test.ts` novo, `readiness.test.ts` reescrito) ·
  tsgo limpo · build OK · lint 0 erros (8 warnings pré-existentes) ·
  Playwright 390×844 OK (card "Estimativa por habilidade" rotulado,
  "confiança baixa" com poucos dados, nenhuma linha mistura alvo com %,
  console limpo). Pesos 20/40/27/13 derivados da matriz oficial
  (`skillMatrix.ts`); `EXAM_WEIGHTS` removido.
  Próxima: Fase 5 (banco: proveniência, duplicatas, payload).
