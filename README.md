# Logpro Projects — Website

Site institucional da Logpro Projects Lda, pronto a publicar no GitHub Pages.

## ⚠️ Importante antes de carregar

Este ZIP já não tem pasta nenhuma lá dentro — o `index.html` e o `README.md`
estão soltos, exatamente como devem ficar na raiz do repositório.

Ao carregar para o GitHub, **arraste os ficheiros individuais**
(`index.html`, `README.md`), nunca uma pasta. Se o GitHub mostrar o
`index.html` dentro de uma subpasta (ex: `logpro-site/index.html`), o
GitHub Pages não o vai encontrar na URL principal e vai dar erro 404.

## O que está incluído

- `index.html` — o site completo (HTML, CSS e JavaScript num único ficheiro autocontido).
  Inclui: seletor de idioma PT/EN, catálogo de produtos com filtros, formulário de
  pedido de cotação ligado ao Formspree, botões de WhatsApp com mensagem
  pré-preenchida, e todo o design responsivo.

Não há mais nenhum ficheiro a carregar — imagens e o serviço de envio de e-mail
(Formspree) estão todos referenciados por URL absoluta, por isso não é preciso
mexer em nada depois de publicar.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (pode ser público ou privado, desde que
   tenha o plano que permite Pages em repositórios privados).
2. Na página principal do repositório, clique em **"Add file" → "Upload files"**.
3. Arraste o `index.html` e o `README.md` **diretamente** para a área de
   upload — não arraste a pasta onde os extraiu, arraste os ficheiros.
4. Confirme, antes de fazer commit, que a lista de ficheiros mostra
   `index.html` e `README.md` soltos (sem nenhuma pasta à frente do nome).
5. Faça o commit ("Commit changes").
6. Vá a **Settings → Pages**.
7. Em **"Branch"**, escolha o branch onde carregou os ficheiros (normalmente
   `main`) e a pasta **`/ (root)`**.
8. Clique em **Save**.
9. Ao fim de 1–2 minutos, o GitHub mostra o link do site publicado, normalmente
   no formato:
   `https://SEU-UTILIZADOR.github.io/NOME-DO-REPOSITORIO/`

## Se aparecer erro 404 "File not found"

Isso quase sempre significa que o `index.html` não está na raiz do
repositório. Abra o repositório no GitHub e confirme que `index.html`
aparece logo na lista principal de ficheiros — se estiver dentro de uma
pasta, mova-o para a raiz (botão **"..."** → **Move file**, ou apague e
carregue de novo sem pasta).

## Depois de publicar

- Teste o formulário de cotação numa página já publicada (https, não file://)
  para confirmar que o envio por AJAX funciona sem interrupções.
- Confirme que o e-mail de verificação do Formspree (para vendas@logpro.co.mz)
  já foi aceite, caso ainda não tenha sido.
- Se mais tarde quiser um domínio próprio (ex: www.logpro.co.mz) em vez do
  domínio github.io, isso configura-se também em Settings → Pages, na secção
  "Custom domain".

## Idioma automático

O site deteta o idioma do navegador do visitante na primeira visita (PT por
omissão, EN se o navegador estiver em inglês) e depois guarda a escolha do
utilizador para as visitas seguintes.
