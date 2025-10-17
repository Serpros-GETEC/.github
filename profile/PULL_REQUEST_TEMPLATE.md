# Título do PR
<!-- Use estilo claro e objetivo. Ex.: feat(area-restrita): habilita login social no fluxo de cadastro -->

## 1) Contexto e Objetivo
<!-- O que motiva este PR? Qual problema resolve? Qual valor de negócio/participante entrega? -->

- Issue vinculada: #<número>  <!-- obrigatória quando houver -->
- Tipo de mudança: 
  - [ ] Feature
  - [ ] Bugfix
  - [ ] Refactor
  - [ ] Chore/Build
  - [ ] Docs
  - [ ] Security/Compliance
  - [ ] Performance

## 2) Escopo da Mudança
<!-- Descreva as principais alterações de código, módulos tocados, limites do que está dentro/fora do PR. -->
- Módulos/Packages tocados:
  - [ ] App (Laravel)
  - [ ] Livewire Components
  - [ ] Blade/Front (Tailwind/Alpine)
  - [ ] Core libs (composer: serpros-getec/*)
  - [ ] Jobs/Queues
  - [ ] API (Controllers/Resources/Policies)
  - [ ] Infra/DevOps (CI/CD, Docker, Helm, Terraform)
  - [ ] Scripts/Tooling

## 3) Detalhes Técnicos
<!-- Liste pontos relevantes para revisão. Inclua decisões e trade-offs. -->
- Padrões/Design Patterns aplicados:
- Endpoints/API alterados (se houver):
  - Método/rota:
  - Contrato (request/response) alterado? [ ] Não [ ] Sim (atualizar OpenAPI)
- Feature flags: [ ] Não [ ] Sim → Nome:
- Migrações de banco: [ ] Não [ ] Sim → `database/migrations/...`
- Seeds/Fixtures: [ ] Não [ ] Sim
- Variáveis de ambiente novas/alteradas: [ ] Não [ ] Sim (documentar em `.env.example`)
- Compatibilidade semântica (libs):
  - Impacta versão? [ ] patch [ ] minor [ ] major
  - Changelog atualizado? [ ] Sim

## 4) Segurança, Privacidade e Conformidade (LGPD)
- Dados pessoais tratados/novos campos? [ ] Não [ ] Sim (descrever minimização/base legal)
- Criptografia/mascaração aplicada quando necessário? [ ] Sim
- Logs não armazenam dados sensíveis (PII/credenciais)? [ ] Confirmado
- Permissões/Policies revisadas (Laravel Gates/Policies): [ ] Sim
- Dependências auditadas (composer/npm): [ ] `composer audit` [ ] `npm audit` OK
- Secret management (OCI Vault/GitHub Secrets) revisado? [ ] Sim

## 5) Performance e Observabilidade
- Impacto de latência/memória/IO: [ ] Baixo [ ] Médio [ ] Alto (detalhar)
- Índices/queries otimizadas? [ ] Sim
- Telemetria/Logs/Métricas (Sentry/ELK/Prometheus) ajustados? [ ] Sim
- Feature possui métricas de sucesso (KPIs/OKRs)? [ ] Sim (quais?)

## 6) Acessibilidade e UX
- Componentes seguem boas práticas (semântica, foco, aria)? [ ] Sim
- Responsividade/Tailwind testada (mobile/desktop): [ ] Sim
- Prints/GIFs:
<!-- Arraste imagens aqui ou use links -->

## 7) Testes
- Cobertura:
  - [ ] Unit (Pest)
  - [ ] Feature (Pest)
  - [ ] Livewire/HTTP
  - [ ] Dusk/E2E (quando aplicável)
- Como testar localmente (passo a passo):
  1. `cp .env.example .env && php artisan key:generate`
  2. `php artisan migrate --seed`
  3. `php artisan serve` (ou Sail) / `npm run dev`
  4. Cenários de teste manual:
     - Caso 1:
     - Caso 2:
- Resultados relevantes (logs/prints):

## 8) Riscos, Rollout e Plano de Reversão
- Riscos identificados:
- Estratégia de rollout:
  - [ ] Deploy canário
  - [ ] Flag de kill-switch
  - [ ] Janela controlada
- Plano de reversão:
  - [ ] `php artisan migrate:rollback` (se houver migração)
  - [ ] Reverter tag/release
  - [ ] Desabilitar feature flag

## 9) Documentação
- README/Docs atualizados? [ ] Sim [ ] N/A
- OpenAPI/Contrato API atualizado? [ ] Sim [ ] N/A
- ADR registrado (se decisão arquitetural): [ ] Sim [ ] N/A

## 10) Checklist de Qualidade (CI/CD)
- [ ] `phpstan`/`larastan` sem erros
- [ ] `php-cs-fixer`/`pint` aplicado
- [ ] `php artisan test` OK
- [ ] `npm run build` OK
- [ ] Pipelines OCI DevOps/GitHub Actions verdes
- [ ] Labels aplicadas (scope, tipo, área)
- [ ] Tamanho do PR razoável (ideal < 500 linhas dif)
- [ ] Review prévia de segurança necessária? [ ] Não [ ] Sim (Security Champion)

## 11) Aprovações
- Revisor técnico (DEV): @
- QA/Teste: @
- Segurança/Privacidade (quando aplicável): @
- Produto/Área demandante (quando aplicável): @

## 12) Itens Relacionados
- PRs dependentes/relacionados:
  - Repositório / PR:
- Tarefas/Issues externas (Jira/Trello/etc. se houver):

---
<!-- Notas para o autor:
1) Mantenha o PR pequeno e focado. Divida em PRs menores quando possível.
2) Aponte o que revisores devem olhar primeiro (arquivos críticos).
3) Use mensagens de commit convencionais (conventional commits) para facilitar versionamento e changelog. -->
