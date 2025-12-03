# Avaliação Institucional – Plataforma de Análise

Projeto desenvolvido pela equipe Mathmorphosis para o Hackathon 2025

## Resumo do Projeto

Este repositório contém a plataforma desenvolvida para análise de dados de avaliações institucionais. O sistema oferece visualizações, filtros por período, métricas consolidadas e comparação entre anos quando aplicável. A aplicação foi construída em Python com o framework Streamlit.

Acesse o projeto:
[https://avaliacaoinstitucionalmath.streamlit.app](https://avaliacaoinstitucionalmath.streamlit.app)

Observação: o site utiliza hospedagem gratuita do Streamlit. Caso esteja offline devido à inatividade, entre em contato pelo número informado no Guia do Avaliador.

## Arquitetura do Projeto

O projeto foi estruturado seguindo princípios S.O.L.I.D e inspirado no padrão MVC, com clara separação de responsabilidades:

### data/

Contém dados brutos (Raw) e processados (Processed), além da lógica de pré-processamento documentada.

### services/

Classes responsáveis pelos cálculos, métricas e regras de negócio.

### view/

Componentes de interface utilizados pelo Streamlit.

### Data Loader

Classe principal responsável por orquestrar o carregamento de dados com segurança. Classe mãe das classes de serviço.

### app.py

Arquivo que orquestra toda a execução da aplicação.

## Execução Local

Para rodar o projeto em sua máquina, siga os passos abaixo:

### Clonar o repositório

Clone o repositório oficial do projeto:

```bash
git clone https://github.com/DEST-UFPR/hackathon-ufpr-IronZiiz.git
```

Acesse o diretório clonado:

```bash
cd hackathon-ufpr-IronZiiz
```

### Criar e ativar um ambiente virtual

Certifique-se de ter o **Python** e o **pip** instalados em sua máquina. Em seguida, crie um ambiente virtual:

```bash
python -m venv venv
```

Ative o ambiente virtual:

* **Windows:**

  ```bash
  venv\Scripts\activate
  ```
* **Linux/Mac:**

  ```bash
  source venv/bin/activate
  ```

### Instalar as dependências

Com o ambiente virtual ativado, instale as dependências necessárias:

```bash
pip install -r requirements.txt
```

### Executar a aplicação

Inicie a aplicação Streamlit:

```bash
streamlit run app.py
```

---

## Participantes

* Thiago
* Gabriel
* Vini


## Observações Sobre Atualização de Dados

Foi considerada uma solução intermediária com uma página para upload de arquivos Excel, permitindo atualização automática dos dados. Essa abordagem não foi totalmente implementada por não ser ideal para escalabilidade, mas o conceito foi documentado.

## Documento Necessário para Avaliação

Para entender completamente o funcionamento, decisões de arquitetura, fluxograma do projeto e instruções detalhadas, o avaliador deve acessar o arquivo **"Guia do Avaliador.pdf"** incluído neste repositório.
