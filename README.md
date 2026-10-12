# Skills

Coleção pessoal de skills para agentes de código (Claude Code e similares), revisadas antes de entrar aqui.

## Como usar

Cada skill é uma pasta com um `SKILL.md`. Copie a pasta para o diretório de skills do seu agente (local ou global) e ele passa a oferecer a skill quando o pedido combinar com a descrição.

## Skills disponíveis

| Skill | Quando usar | Para que serve |
|---|---|---|
| [web-design-guidelines](web-design-guidelines) | Pedidos como "revisar minha UI", "checar acessibilidade", "auditar design" ou "revisar UX" | Revisa código de interface contra as Web Interface Guidelines (padrões visuais e de interação), apontando os problemas no formato arquivo:linha |
| [the-judge](the-judge) | Antes de abrir ou subir um PR, para revisar o diff como um revisor sênior (ou pedindo "revise esse PR", "julgue esse PR") | Avalia o PR exigindo evidência para cada apontamento (correção, segurança, qualidade estrutural, código gerado por IA) e posta uma única revisão consolidada no GitHub via `gh` CLI, com veredito APPROVE, COMMENT ou REQUEST_CHANGES |

## Créditos

Skill de terceiro mantém o autor original no campo `metadata.author` do `SKILL.md` e, quando aplicável, a licença de origem.
