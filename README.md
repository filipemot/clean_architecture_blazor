
# Blazor - Clean Architecture 

Projeto de um Catálogo de Produtos de Beleza - Aplicação de Clean Architecture com Blazor

Baseado as vídeo aulas do Macoratti

**Camadas do projeto**

**Camada Core**

Camada de domínio onde teremos as **entidades e as regras de negócio do projeto**. É um projeto **Class Library**;

**Camada UseCases**

Camada da aplicação representando **os casos de uso** para mostrar o catálogo, procurar um produto e exibir os detalhes do produto. É um projeto **Class Library**;

**Camada Data**

Camada de infraestrutura, onde vamos definir o **acesso aos dados** representado pelo repositório. É um projeto **Class Library**;


**Camada Data**

Camada de interface onde vamos criar os **componentes Blazor** é representada pelo projeto **Blazor Server**

**Dependências**

 - Core - **Nenhuma**
 - UseCases - **Core**
 - Data - **UsesCases**
 - Blazor - **Core, UseCases, Data**
