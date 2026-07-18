# PWA — Formulário da Igreja do Nazareno em Tchumene

## Formulário ligado

https://ee-eu.kobotoolbox.org/x/phsELa2l

## Ficheiros

- `index.html`: página que será enviada aos utilizadores;
- `manifest.webmanifest`: identidade e configuração da PWA;
- `service-worker.js`: instalação e funcionamento básico sem ligação;
- `offline.html`: mensagem apresentada quando não há Internet;
- `emblema-completo.png`: emblema apresentado na página;
- `icons/`: ícones Android, iPhone e maskable;
- `vercel.json`: cabeçalhos recomendados para publicação no Vercel.

## Publicação no Vercel como projecto separado

1. Crie um repositório GitHub.
2. Coloque todos os ficheiros desta pasta na raiz do repositório.
3. No Vercel, seleccione **Add New → Project**.
4. Importe o repositório.
5. Em Framework Preset, seleccione **Other**.
6. Não indique Build Command.
7. Publique.
8. Envie aos utilizadores o domínio fornecido pelo Vercel.

## Publicação dentro de um projecto já existente

Copie a pasta para uma rota pública do projecto, por exemplo:

`formulario-tchumene/`

Depois, o link será semelhante a:

`https://SEU-DOMINIO/formulario-tchumene/`

Como os caminhos do manifesto e do Service Worker são relativos, a PWA funciona também numa subpasta. Nesse caso, não copie o `vercel.json` desta pasta para substituir uma configuração já existente sem primeiro integrar os respectivos cabeçalhos.

## Teste

1. Abra o link publicado num telefone Android com Chrome.
2. Aguarde alguns segundos.
3. Toque em **Instalar no telefone**.
4. Confirme que aparece no ecrã principal com o emblema da Igreja.
5. Abra o ícone e toque em **Abrir formulário**.

No iPhone/iPad:

1. Abra no Safari.
2. Toque em **Partilhar**.
3. Seleccione **Adicionar ao ecrã principal**.
