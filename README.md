# Carteira — Rebalanceador

App de página única para acompanhar carteiras de investimento e dividir o aporte
do mês entre os ativos mais distantes da posição-alvo.

## Publicar no GitHub Pages

1. Crie um repositório (pode ser privado; o Pages de repositório privado exige
   conta paga — para conta grátis, use um repositório público).
2. Envie **todos** os arquivos desta pasta para a raiz do repositório.
3. No repositório: **Settings → Pages**. Em *Source*, escolha `Deploy from a branch`,
   selecione a branch `main` e a pasta `/ (root)`. Salve.
4. Em um ou dois minutos o endereço aparece na mesma tela, no formato
   `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Instalar no celular

Abra esse endereço no navegador do celular e use **Adicionar à Tela de Início**
(no iPhone, pelo botão de compartilhar do Safari). O app passa a abrir em tela
cheia, com ícone próprio, e funciona sem internet.

## Levar seus dados para cá

Os dados **não** vêm junto com os arquivos: eles ficam guardados no navegador de
cada aparelho. Para transferir:

1. Na versão antiga do app, abra o menu **⋯** ao lado das abas e escolha
   **Exportar dados (backup)**. Toque em *Copiar tudo*.
2. Guarde esse texto onde você conseguir abrir no celular (e-mail para si mesmo,
   bloco de notas sincronizado, arquivo no Drive).
3. Abra esta versão no celular, menu **⋯** → **Importar dados**, cole e confirme.

Faça o mesmo caminho de tempos em tempos como backup: aqui os dados ficam no
armazenamento do navegador, e some se você limpar os dados do site ou trocar de
aparelho.

## Atualizar o app

Substitua o `index.html` no repositório. O service worker busca a rede primeiro,
então a versão nova chega na abertura seguinte. Se quiser forçar, troque o nome
do cache em `sw.js` (`carteira-v1` → `carteira-v2`).

## Arquivos

| Arquivo | Para que serve |
|---|---|
| `index.html` | O app inteiro: interface, cálculos, lista de ativos |
| `manifest.json` | Nome, cores e ícones ao instalar na tela de início |
| `sw.js` | Service worker: faz abrir offline |
| `icon-*.png`, `apple-touch-icon.png` | Ícones |

Ferramenta de organização pessoal. Não é recomendação de investimento.
