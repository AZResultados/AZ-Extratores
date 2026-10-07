---
projeto: AZ-Extratores
vertical: Institucional
status: Parado
status_desde: 2026-05-10
manutencao: não
revisado_em: 2026-09-15
trava: James — sem data de retomada definida
---

# Estado — AZ-Extratores

## Aberto

- Definir data de retomada — depende de: James. ⚠️ Gatilho de 90 dias de `Parado` já vencido em 08/08/2026: rodar o diagnóstico 1.1 do `JW-Org\CLAUDE.md` ou registrar a data aqui.

- Atualizar o `BASE_DIR` nas planilhas `.xlsm` que já importaram o `ModConfig.bas` (reimportar o módulo de `vba\`) — a cópia dentro da planilha não muda sozinha — depende de: James
- Decidir se o projeto muda de nome: "Extratores" promete mais do que o produto faz (fatura de cartão em PDF) — depende de: James

## Estado

- ⚠️ `vba\ModConfig.bas` guarda o caminho absoluto do projeto em `BASE_DIR`. Mover ou renomear a pasta exige corrigir a constante, reimportar o módulo nas planilhas e recriar o `venv\`. O Python não tem caminho fixo (`EXTRATORES_DB` e `__file__`); o banco fica em `~\.extratores\dados.db`, fora do projeto.
- Parsers Python de fatura/extrato com integração VBA/Excel. James declarou em 15/09/2026 que vai retomar. Arquitetura e extratores concluídos em `README.md` e `docs\`.

## Histórico

| Data | O que mudou |
|---|---|
| 2026-10-07 | Pasta movida para o envelope `Institucional\AZ-Conectores\` por decisão de James. `BASE_DIR` do `ModConfig.bas` corrigido (apontava para `C:\Dev\projetos\Extratores`, caminho anterior às verticais), `venv\` recriado, 93/93 testes passando no caminho novo. Status segue `Parado`. |
| 2026-09-15 | Status `Parado` (com retomada prevista) decidido por James na formalização de 15/09/2026. |
| 2026-05-10 | Último commit. |
