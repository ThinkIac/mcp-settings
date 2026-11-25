# mcp

Global configuration and discovery of Model Context Protocol providers.

Repositório: https://github.com/ThinkIac/mcp-settings.

## Uso no ThinkIac

Este pacote foi extraído de `packages/mcp`. Preserve a identidade `mcp` do manifest ao instalá-lo em um workspace Lógos. Views, rotas, ferramentas e hooks são descobertos pelo runtime e dependem dos provedores correspondentes. Esta extração publica o código atual; não converte JavaScript para LógosType nem implementa instalação por perfil.

Entrada declarada: `index.js`.

## Dependências e validação

Consulte `package.json` e os imports para as capacidades exigidas do host.

Scripts disponíveis: `npm run test`.

## Segurança e dados locais

Credenciais devem ser configuradas no ambiente de destino. Não acompanham esta extração bancos, sessões, uploads, perfis pessoais, arquivos `.env`, caches ou backups. As exclusões foram registradas em relatório externo à publicação. Configure segredos pelo host, sem incluí-los em commits.


## Registros encontrados no código

- `router`: `providers`, `providers/:name`, `providers/:name/refresh`, `system/action`, `system/view`.

A lista é um inventário estático e pode incluir registros em testes; não garante disponibilidade sem os provedores do host.

Há imports relativos para diretórios superiores. A instalação isolada e a composição por perfil precisam resolver esses vínculos antes de remover a cópia da base.

