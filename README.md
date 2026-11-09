# MAX OBRA

Site público da loja de materiais de construção, com catálogo, orçamento pelo WhatsApp, consulta de frete e solicitação de entrega.

## Publicar pelo GitHub e pela Vercel

1. Crie um repositório GitHub chamado `max-obra-site`. Use um repositório privado se quiser que apenas sua equipe veja o código.
2. Extraia este pacote. Envie o conteúdo da pasta extraída para a raiz do repositório, incluindo a pasta `dist` e o arquivo `vercel.json`.
3. Na Vercel, entre na equipe com plano compatível com uso comercial e importe `max-obra-site` em **Add New → Project**. Autorize o acesso a esse repositório no GitHub.
4. Mantenha a raiz do projeto como está. O arquivo `vercel.json` já aponta para `dist` e desativa as etapas de instalação e compilação. Clique em **Deploy**.
5. Abra o endereço fornecido pela Vercel em uma aba anônima. Confira catálogo, menu no celular, frete e abertura da mensagem de orçamento no WhatsApp.

O plano Hobby da Vercel é para uso pessoal e não comercial. Consulte [a documentação da Vercel](https://vercel.com/docs/plans/hobby).

## Testar no computador

Na pasta do projeto, rode `python -m http.server 8000 --directory dist` e acesse `http://localhost:8000`. O catálogo usa HTTP para carregar o arquivo JSON.

O site é estático. O catálogo fica em `dist/catalog.json`. Depois que o repositório estiver conectado, atualizações na branch de produção da Vercel geram uma nova publicação.
