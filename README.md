# Missão Aquário Digital

Protocolo de Versionamento e Gestão de Ecossistema — atividade da disciplina de Garantia da Qualidade de Software / Gestão e Qualidade de Software.

## Sobre o projeto

O **aquario-digital-core** simula o ecossistema de desenvolvimento de um sistema de controle e monitoramento de um aquário digital, praticando um fluxo de versionamento corporativo com três camadas de ambiente.

## Camadas do ambiente

| Branch | Papel | Descrição |
|---|---|---|
| `main` | Produção | Código estável, validado e pronto para uso em produção. |
| `stage` | Homologação / Testes | Ambiente intermediário onde as funcionalidades vindas da `develop` são testadas antes de seguir para produção. |
| `develop` | Desenvolvimento | Branch de integração das novas funcionalidades, criadas a partir de branches `feature/*`. |

Fluxo de integração: `feature/*` → `develop` → `stage` → `main`

## Módulo: Controle de Qualidade da Água

Classe `ControleQualidadeAgua.java`, desenvolvida na branch `feature/controle-qualidade`, responsável por monitorar os parâmetros essenciais para a saúde do aquário:

- **pH**: nível ideal entre 6.8 e 7.6
- **Temperatura**: nível ideal entre 22.0°C e 28.0°C

O método `verificarParametros()` valida os dois parâmetros e emite alertas de QA quando algum valor está fora da faixa segura.

## Equipe

**Biólogos/Desenvolvedores responsáveis:**

- Leandro Cavalcante

## Disciplina

- **Curso:** Garantia da Qualidade de Software / Gestão e Qualidade de Software
- **Professor:** Daniel Henrique Matos de Paiva