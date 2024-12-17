# Neon Theme para Magento

**Versão**: 1.0  
**Data de Atualização**: 05/2021
**Desenvolvedor**: Nilson Junior

## Descrição

O **Neon Theme** é um conjunto de funções desenvolvidas para melhorar a experiência do usuário e otimizar a interface de um **tema Magento**. Essas funções adicionam interatividade e aprimoram a usabilidade da loja, incluindo ajustes de layout, animações dinâmicas, e correções para navegadores antigos. 

Este script é projetado para personalizar o comportamento e a aparência da loja Magento, implementando recursos como carrosséis de produtos, ajustes de categorias, correções de SVG para navegadores antigos, e muito mais.

## Funcionalidades

As funções descritas abaixo podem ser utilizadas para personalizar o tema de sua loja Magento:

### 1. **Função `dropFrom()`**

Gerencia a exibição de elementos interativos como menus e filtros, ajustando o comportamento deles conforme a rolagem ou redimensionamento da página. A função é aplicada em elementos como:
- `.mywish`
- `.mycart`
- `.myaccount`
- `.categories:not(.categories--carrossel) .li--0`
- `.search__filter`

### 2. **Função `fix_IE_SVGs()`**

Corrige a exibição de ícones SVG em versões antigas do **Internet Explorer**, garantindo que todos os ícones gráficos sejam corretamente renderizados nesse navegador.

### 3. **Função `default_categories_justify()`**

Ajusta a justificação das categorias na página, garantindo que o layout seja organizado de forma responsiva, seja em desktop ou dispositivos móveis.

### 4. **Função `default_categories_mini()`**

Aplica um layout simplificado para as categorias, criando uma visualização limpa e eficiente, ideal para lojas com um grande número de categorias.

### 5. **Função `default_carrossel_produtos()`**

Ativa um carrossel de produtos, permitindo a exibição de itens de forma interativa e rolável na página. Ideal para destacar produtos em promoção ou lançamentos.

### 6. **Função `fix_zoomHeader()`**

Corrige o comportamento de zoom no cabeçalho da loja, melhorando a visualização para usuários em dispositivos móveis ou com telas sensíveis ao toque.

### 7. **Função `addSVG()`**

Adiciona ícones SVG em locais estratégicos, como:
- Status de pedidos (novo, processando, enviado)
- Redes sociais (Facebook, Twitter, Google+, LinkedIn)
- Ícones de visualização de produtos (grelha ou lista)

Os ícones podem ser configurados para serem inseridos antes ou depois do conteúdo (usando `prepend` ou `append`).

### 8. **Função `default_categories_carrossel()`**

Ativa um carrossel para exibir as categorias de forma interativa, proporcionando uma navegação agradável e dinâmica para os usuários.

### 9. **Função `default_carrossel_brands()`**

Exibe um carrossel de marcas, permitindo destacar marcas populares ou parceiras da loja.

### 10. **Função `default_carrossel_jointsales()`**

Ativa um carrossel para promover vendas conjuntas, oferecendo pacotes de produtos ou promoções combinadas de forma interativa.

### 11. **Função `default_carrossel_home()`**

Ativa o carrossel na página inicial, permitindo a exibição de produtos ou promoções de forma dinâmica e interativa.

### 12. **Função `fix_category_description()`**

Corrige a exibição da descrição das categorias para garantir que o conteúdo seja visualizado corretamente em todas as resoluções de tela.

### 13. **Função `default_tabs()`**

Adiciona abas interativas em várias seções do site, permitindo que o conteúdo seja organizado em categorias acessíveis de forma rápida e eficiente.

### 14. **Função `fix_address_phone()`**

Corrige a exibição dos campos de endereço e telefone, melhorando a usabilidade durante o processo de checkout, especialmente em dispositivos móveis.

## Como Usar

1. **Integrar no Tema Magento**:
   Para usar o Neon Theme, basta adicionar o script ao seu tema Magento, geralmente no arquivo `theme.js` ou diretamente nas templates.

2. **Configuração Personalizada**:
   Você pode configurar as funcionalidades do Neon Theme através de um objeto de opções. Exemplo de uso:

   ```javascript
   $('.element').neonTheme({
       default_dropFrom: true,
       fix_IE_SVGs: true,
       default_carrossel_produtos: true
   });
