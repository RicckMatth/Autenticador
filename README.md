# Autenticador — Chrome (sem compactação)

<div align="center">

<a href="https://github.com/RicckMatth/Autenticador/archive/refs/heads/main.zip">
  <img src="assets/botao-download.svg" alt="⬇ BAIXAR AUTENTICADOR PARA CHROME — DOWNLOAD DIRETO ZIP" width="720">
</a>

**Clique no botão acima para baixar o ZIP diretamente do GitHub.** Depois de extrair, selecione a pasta que contém o arquivo `manifest.json` em `chrome://extensions` → **Carregar sem compactação**.

</div>

Repositório de distribuição **da versão oficial compilada do Authenticator Extension v8.0.2**, destinada a instalação local no Google Chrome pelo recurso **Carregar sem compactação**.

**Projeto original:** https://github.com/Authenticator-Extension/Authenticator  
**Release de origem:** https://github.com/Authenticator-Extension/Authenticator/releases/tag/v8.0.2  
**Licença original:** MIT — arquivo [LICENSE](LICENSE)

> Este é um espelho de distribuição não oficial e **não** uma publicação dos mantenedores. Os arquivos compilados vêm do pacote oficial `release.tar.gz`, sem modificações intencionais.

## Como instalar no Chrome

1. Clique no **botão verde BAIXAR AUTENTICADOR** no topo desta página.
2. Extraia o ZIP para uma pasta fixa. **Não** carregue o ZIP diretamente.
3. Abra `chrome://extensions` no Chrome.
4. Ative **Modo do desenvolvedor**, caso essa opção seja permitida.
5. Clique em **Carregar sem compactação**.
6. Selecione a **pasta extraída que contém `manifest.json`**, e não uma subpasta como `dist`.

A extensão utiliza `manifest.json` (Manifest V3), `dist/`, `css/`, `view/`, `images/` e `_locales/`. **Não apague nenhuma dessas pastas.**

## Atualização / origem dos arquivos

O fluxo [publicar-chrome.yml](.github/workflows/publicar-chrome.yml) baixa o arquivo de release diretamente do projeto original, verifica a estrutura e publica **somente os arquivos da distribuição Chrome** na raiz deste repositório. Ele pode ser iniciado manualmente pela aba **Actions**.

## Importante

- **Não** há garantia de que esta instalação funcione em máquinas gerenciadas: políticas corporativas podem impedir extensões locais. Siga as regras e orientações de TI da empresa.
- Esta cópia pode ter **ID de extensão diferente** da versão da Chrome Web Store. Recursos que dependem desse ID, incluindo algumas integrações de login/backup, podem precisar de configuração adicional e não são garantidos.
- Não desinstale uma versão existente com contas cadastradas sem **validar antes um backup recuperável** dos seus códigos 2FA.
- Nunca publique segredos OTP, backups de contas, QR Codes de autenticação nem senhas neste repositório.
