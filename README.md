
# Scraping de Questões de Exames

Este projeto é uma ferramenta de scraping para extrair questões de exames, com foco em ENEM e concursos. Utilizando o site [QConcursos](https://www.qconcursos.com/), a aplicação permite a filtragem e visualização de questões com base em diversos critérios.

## Funcionalidades

- **Scraping de Questões**: Coleta automatizada de questões de exames.
- **Filtros Avançados**: Filtragem de questões por disciplina, assunto, dificuldade e ano de publicação.
- **Interface Interativa**: Interface desenvolvida com Streamlit para visualização e interação.
- **Duas Páginas Específicas**:
  - **Concursos**: Focada em questões de diversos concursos.
  - **ENEM**: Especializada em questões do ENEM.

## Tecnologias Utilizadas

- **Streamlit**: Para criar a interface interativa.
- **BeautifulSoup**: Para parsing e extração de dados das páginas web.
- **Requests**: Para realizar requisições HTTP.

## Como Funciona

### 1. **Configuração do Ambiente**

Clone o repositório e instale as dependências:

```sh
git clone git@github.com:victormalvao/scraping-questoes-concursos.git
cd scraping-questoes-concursos
pip install -r requirements.txt
```

### 2. **Executar o Aplicativo**

Para iniciar o aplicativo, execute:

```sh
streamlit run main.py
```

### 3. **Uso do Aplicativo**

**Página de Concursos:**

- **Seleção de Disciplinas**: Escolha as disciplinas para as quais deseja obter questões.
- **Seleção de Assuntos**: Escolha os assuntos relevantes dentro das disciplinas selecionadas.
- **Nível de Dificuldade**: Defina a dificuldade das questões.
- **Anos de Publicação**: Escolha os anos para filtrar as questões.
- **Número Máximo de Páginas**: Defina quantas páginas de resultados deseja extrair.

**Página do ENEM:**

- **Seleção de Disciplinas e Assuntos**: Similar ao filtro de concursos, mas especializado para questões do ENEM.

### 4. **Filtragem Detalhada**

A filtragem permite uma busca refinada com base nos seguintes critérios:

- **Disciplinas**: Escolha entre uma lista de disciplinas para limitar o escopo das questões.
- **Assuntos**: Após selecionar as disciplinas, escolha assuntos específicos para obter questões mais direcionadas.
- **Nível de Dificuldade**: Filtre questões de acordo com a dificuldade desejada (Muito Fácil, Fácil, Médio, Difícil, Muito Difícil).
- **Anos de Publicação**: Selecione o intervalo de anos para filtrar as questões de acordo com a data de publicação.
- **Número Máximo de Páginas**: Controle quantas páginas de resultados você deseja extrair, com um valor máximo configurável.

### 5. **Detalhes Técnicos**

A função principal da aplicação é construir a interface e a lógica para realizar o scraping das questões. O código para isso é estruturado da seguinte forma:

- **Título e Descrição**: Fornece um resumo sobre o propósito do aplicativo.
- **Instância das Classes**: Cria instâncias das classes `QConcursosAPI` e `URLBuilder` para realizar a extração e construção de URLs.
- **Carregamento e Seleção de Disciplinas e Assuntos**: Obtém e apresenta opções para que o usuário selecione os filtros desejados.
- **Geração da URL**: Cria a URL de busca com base nos filtros selecionados e realiza o scraping.
- **Exibição dos Resultados**: Mostra as questões extraídas em um formato organizado, com opções para visualizar detalhes e alternativas.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).



