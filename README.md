# Galeria de Doces

Site estático de uma doceria, com uma galeria de doces em cartões no estilo polaroid. Ao selecionar um cartão, a página exibe uma tela padrão de detalhes e um formulário de solicitação de encomenda.

## Funcionalidades

| Funcionalidade | Descrição |
| --- | --- |
| Galeria de doces | Apresenta 12 opções de doces com fotos e legendas em uma grade responsiva. |
| Navegação para detalhes | Cada polaroid abre a página padrão de detalhes com o nome e a imagem do doce selecionado. |
| Informações do produto | Exibe uma descrição genérica e o preço como “Sob consulta”, para personalização posterior. |
| Formulário de encomenda | Permite preencher nome, quantidade e contato. Ao enviar, mostra uma confirmação na própria página. |
| Layout adaptável | Ajusta a grade da galeria e a disposição da página de detalhes para telas menores. |

## Sobre a organização do código

`SiteDoces.html` contém a galeria e um pequeno trecho de JavaScript que passa o nome e a imagem do doce selecionado para a página de detalhes pela URL. `DocesEstilo.css` concentra a aparência da galeria, incluindo a grade, o estilo polaroid e os ajustes para telas menores.

`detalhes.html` usa os dados recebidos pela URL para preencher o nome e a imagem do produto. A descrição e o preço são textos genéricos que podem ser atualizados para cada doce. `detalhes.css` mantém os estilos da página de detalhes separados dos estilos da galeria. A imagem `fundo.jpeg` é usada como fundo nas duas páginas; as fotos dos doces são carregadas de URLs do Unsplash.

Essa divisão mantém separadas a estrutura das páginas e suas regras visuais, enquanto o JavaScript simples reaproveita uma única página de detalhes para todos os cartões.

## Navegação entre páginas com parâmetros

Ao clicar em uma polaroid, o JavaScript lê o nome e o endereço da imagem no próprio cartão e os acrescenta à URL de `detalhes.html`. A página de detalhes consulta esses parâmetros para mostrar o produto escolhido sem criar uma página HTML diferente para cada doce.

O formulário demonstra a interação e exibe uma confirmação local após o envio. Ele ainda não encaminha os dados para a doceria.

## Aprendizados aplicados

- Estruturação de páginas com HTML semântico, links, imagens e formulários.
- Separação dos estilos em folhas CSS externas.
- Uso de CSS Grid e media queries para organizar o conteúdo em diferentes larguras de tela.
- Uso de parâmetros de URL para compartilhar dados entre páginas.
- Manipulação do conteúdo da página e tratamento do envio de formulário com JavaScript.
- Uso de texto alternativo nas imagens para descrever seu conteúdo.
