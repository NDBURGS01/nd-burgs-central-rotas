# ND BURGS — GitHub Pages

Site público de entrada do sistema ND BURGS. A interface operacional, autenticação, pedidos, GPS e dados permanecem no Google Apps Script/Google Sheets. O site carrega a implantação existente do Apps Script e encaminha os links públicos de pedido/mapa.

## Endereços já configurados

- Repositório: https://github.com/NDBURGS01/nd-burgs-central-rotas
- Site: https://ndburgs01.github.io/nd-burgs-central-rotas/
- Apps Script: https://script.google.com/macros/s/AKfycbz2SRJUvUocGtGoCMZSKL3isp51CPhe5K-ChmNlQC7Y7mhwQ9L3zzts_QRTdErY6KkH/exec

## Publicar o site

1. Extraia este pacote.
2. Envie o CONTEÚDO desta pasta para a raiz do repositório `NDBURGS01/nd-burgs-central-rotas` (index.html precisa ficar na raiz; não envie apenas o ZIP).
3. Faça Commit na branch `main`.
4. No GitHub, abra Settings → Pages.
5. Em Build and deployment, escolha `Deploy from a branch`, branch `main`, pasta `/ (root)` e salve.
6. Aguarde o GitHub Pages publicar o endereço indicado acima.

## Conectar o Apps Script (pacote privado separado)

O arquivo `Code.gs` do pacote privado ND_BURGS_APPS_SCRIPT_GITHUB.zip já está configurado para gerar links públicos usando o domínio GitHub Pages e já contém `ALLOWALL` na função `doGet`.

No projeto Google Apps Script, mantenha os arquivos com os nomes exatos `Code.gs`, `Index.html` e `LocationMap.html`. Faça backup do projeto atual antes de substituir. Depois salve e publique uma nova versão do Web App, mantendo a implantação acessível conforme a configuração já utilizada.

**Não coloque o pacote privado do Apps Script no GitHub público.** Ele contém configurações internas e PINs de acesso. Publique somente os arquivos deste pacote GitHub Pages.

## Testes obrigatórios após publicar

- Abrir o site no computador e no celular.
- Entrar como administrador.
- Entrar com um acesso de motoboy.
- Conferir pedidos e atualização de status.
- Conferir geração e abertura de links `?pedido=` e `?mapa=`.
- Conferir permissão de localização GPS.

## Instalação no celular

Depois que o GitHub Pages estiver publicado, abra o endereço no Android e use a opção de instalar/adicionar à tela inicial. No iPhone, abra no Safari → Compartilhar → Adicionar à Tela de Início.

O navegador precisa permanecer ativo e com permissão de localização para enviar GPS. Atualização contínua com tela bloqueada não é garantida por uma página web.
