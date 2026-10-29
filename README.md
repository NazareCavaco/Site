# Apiserpa — Site de Apicultura e Catálogo de Produtos

Site desenvolvido em **HTML e CSS** para apresentar a Apiserpa, divulgar informação sobre a empresa e disponibilizar um catálogo de mel e outros produtos apícolas.

O projeto reúne uma página inicial, uma apresentação da empresa, um catálogo com imagens e preços, páginas de detalhe de produtos e uma página de contactos. Demonstra a construção de um site com várias páginas e uma identidade visual comum.

## Funcionalidades

- Navegação entre Início, Sobre Nós, Contactos e Produtos.
- Página inicial com imagens relacionadas com apicultura.
- Apresentação da história da empresa.
- Catálogo com imagens, quantidades e preços apresentados no projeto.
- Páginas de detalhe para mel de rosmaninho e mel multifloral, em embalagens de 500 g e 1 kg.
- Página de contactos com informação da empresa e estrutura de formulário.
- Rodapé com navegação e ligações para redes sociais.
- Efeitos de interação nos cartões dos produtos através de CSS.

**Âmbito:** trata-se de um site de apresentação e catálogo. Não inclui carrinho de compras, pagamentos, autenticação ou base de dados. O formulário de contacto requer ajustes antes de ser utilizado.

## Tecnologias utilizadas

| Tecnologia | Utilização |
| --- | --- |
| HTML5 | Estrutura e conteúdo das páginas. |
| CSS3 | Cores, tipografia, espaçamentos, efeitos e organização visual. |
| Flexbox | Distribuição de elementos e organização em colunas. |
| Media queries | Regras de adaptação do layout a ecrãs mais pequenos. |
| Google Fonts | Carregamento da fonte Poppins. |
| JavaScript | Código preliminar de envio de email na página de contactos. |

A página de contactos contém referências ao FormSubmit e ao SMTPJS, mas a integração de envio de mensagens está incompleta.

## Como abrir o projeto

1. Descarrega e extrai o ZIP do repositório.
2. Abre a pasta que contém `index.html`.
3. Abre `index.html` num navegador.

Não é necessário instalar dependências, compilar o projeto ou configurar uma base de dados. Mantém os ficheiros HTML, CSS e as imagens nas respetivas localizações.

A ligação à Internet é necessária para carregar a fonte do Google Fonts e os serviços externos referenciados. Os problemas de caminhos indicados abaixo podem impedir a apresentação de algumas imagens e a navegação por certas ligações.

### Servidor local opcional

Se tiveres Python 3 instalado, podes iniciar um servidor na pasta do projeto:

```bash
python -m http.server 8000
```

Em sistemas onde o comando é `python3`, utiliza:

```bash
python3 -m http.server 8000
```

Depois, abre [http://localhost:8000](http://localhost:8000). Para terminar o servidor, utiliza `Ctrl + C` no terminal.

## Estrutura do projeto

| Ficheiro | Descrição |
| --- | --- |
| `index.html` | Página inicial. |
| `sobre.html` | Apresentação e história da empresa. |
| `produtos.html` | Catálogo de produtos. |
| `contactos.html` | Informação de contacto e formulário. |
| `rosmaninho1.html` | Detalhe do mel de rosmaninho de 1 kg. |
| `rosmaninho500.html` | Detalhe do mel de rosmaninho de 500 g. |
| `multifloral1.html` | Detalhe do mel multifloral de 1 kg. |
| `multifloral500.html` | Detalhe do mel multifloral de 500 g. |
| `style.css` | Estilos partilhados pelas páginas. |
| Ficheiros `.png` e `.jpg` | Logótipos, imagens de produtos e ícones. |
| `LICENSE` | Licença incluída no repositório. |

## Competências demonstradas

- Criação e ligação de várias páginas HTML.
- Separação entre conteúdo e apresentação através de CSS externo.
- Organização de catálogos e páginas de detalhe.
- Aplicação de Flexbox, media queries e efeitos de hover.
- Construção visual de formulários.
- Integração de imagens, tipografia e navegação numa interface comum.

## Estado atual e melhorias previstas

Esta versão contém alguns pontos a rever:

- **Caminhos das imagens:** algumas páginas usam `./imagens/`, mas no ZIP as imagens encontram-se na pasta principal. É necessário uniformizar os caminhos.
- **Ligações de navegação:** existem referências a `site.html` e `index.php`, que não estão incluídos. As ligações para a página inicial devem apontar para `index.html`.
- **Detalhes dos produtos:** alguns artigos do catálogo apontam para uma página de outro produto.
- **Formulário:** faltam atributos `name` nos campos e existem atributos `type` malformados. O código SMTPJS contém valores de exemplo e a função não está ligada à submissão do formulário. É necessário concluir e testar uma única solução de envio; credenciais SMTP não devem ser colocadas no código público.
- **Adaptação a dispositivos móveis:** rever o menu, o formulário e adicionar a configuração de viewport às páginas.
- **Acessibilidade e conteúdo:** adicionar texto alternativo às imagens, associar etiquetas aos campos, rever os textos e substituir as ligações genéricas das redes sociais.

## Licença

O repositório inclui a **GNU General Public License v3.0**. Consulta o ficheiro [LICENSE](LICENSE) para conhecer os termos.
