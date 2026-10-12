# Skills

Coleção pessoal de skills para agentes de código (Claude Code e similares), revisadas antes de entrar aqui.

## Como usar

Cada skill é uma pasta com um `SKILL.md`. Copie a pasta para o diretório de skills do seu agente (local ou global) e ele passa a oferecer a skill quando o pedido combinar com a descrição.

## Skills disponíveis

| Skill | Quando usar | Para que serve |
|---|---|---|
| [web-design-guidelines](web-design-guidelines) | Pedidos como "revisar minha UI", "checar acessibilidade", "auditar design" ou "revisar UX" | Revisa código de interface contra as Web Interface Guidelines (padrões visuais e de interação), apontando os problemas no formato arquivo:linha |
| [the-judge](the-judge) | Antes de abrir ou subir um PR, para revisar o diff como um revisor sênior (ou pedindo "revise esse PR", "julgue esse PR") | Avalia o PR exigindo evidência para cada apontamento (correção, segurança, qualidade estrutural, código gerado por IA) e posta uma única revisão consolidada no GitHub via `gh` CLI, com veredito APPROVE, COMMENT ou REQUEST_CHANGES |
| [web-accessibility](web-accessibility) | Pedidos como "melhorar acessibilidade", "auditoria de a11y", "conformidade com WCAG" ou "suporte a leitor de tela" | Audita e melhora acessibilidade de HTML/CSS seguindo WCAG 2.1 (navegação por teclado, leitor de tela, contraste), com checklist baseado nos critérios do Lighthouse |
| [web-quality-audit](web-quality-audit) | Pedidos como "auditar meu site", "revisar qualidade da página" ou "rodar auditoria Lighthouse", quando quer performance, acessibilidade, SEO e boas práticas de uma vez | Orquestra uma auditoria completa ao estilo Lighthouse (mais de 150 verificações), cobrindo performance, acessibilidade, SEO e boas práticas em uma única revisão |

## Créditos

Skill de terceiro mantém o autor original no campo `metadata.author` do `SKILL.md` e, quando aplicável, a licença de origem.
