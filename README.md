# Análise dos relatórios de auditoria

#### UFPB - Universidade Federal da Paraíba
#### LabGov
Autores: Bruno Souza da Costa e Cecília Lori de Medeiros Cruz  


bruno.souza@dcx.ufpb.br  
cecilia.medeiros@dcx.ufpb.br

### Esse código foi utilizado para realizar as análises de dados sobre os relatórios de auditoria interna governamental e os critérios do manual do TCU cumpridos por estes

Serão realizadas diversas análises com a finalidade de representar melhor os dados e responder às seguintes questões:

- Quantos e qual a porcentagem dos casos por unidade da federação?
- Quantos e qual a porcentagem dos casos por tipo do relatório?
- Quantos e qual a porcentagem dos casos pelo ano de publicação do relatório?
- Quantos e qual a porcentagem dos casos por região?
- Quantos e qual a porcentagem dos casos mensais de cada ano?
- Quantos e qual a porcentagem dos casos antes, durante e depois da pandemia?
- Quantos e qual a porcentagem dos casos por governo vigente?
- Qual a porcentagem dos critérios por unidade da federação?
- Qual a porcentagem dos critérios por tipo do relatório?
- Qual a porcentagem dos critérios por ano de publicação do relatório?
- Qual a porcentagem dos critérios por região?
- Qual a porcentagem dos critérios mensalmente de cada ano?
- Qual a porcentagem de correlação entre esses critérios?

## 🗂️ **Estrutura do Projeto**

```bash
├── .github/                         # Contém configurações para GitHub Actions
|    └── workflows/
|        └── deploy-docs.yml         # Workflow para deploy automático da análise
|
├── Gráficos/                        # Pasta onde os gráficos gerados são armazenados
├── Tabelas/                         # Pasta onde as tabelas geradas são armazenadas
|
├── .gitignore                       # Controla arquivos e diretorios que podem ser versionados
├── analisador_auditoria.ipynb       # Arquivo onde análises são realizadas
├── README.md                        # Este arquivo
├── relatorios.csv                   # Banco de dados utilizado para as análises
└── requirements.txt                 # Contém todas as bibliotecas python necessárias para funcionamento
```

## **Pré-requisitos**

Certifique-se de que seu sistema possui as seguintes ferramentas instaladas:

* **Python 3.8+**: Linguagem de programação principal do projeto.
    * Verifique com: `python3 --version`
* **pip**: Gerenciador de pacotes do Python (geralmente vem com o Python).
    * Verifique com: `pip3 --version`
* **Git**: Sistema de controle de versão, essencial para clonar o repositório.
    * Verifique com: `git --version`
* **VSCode**: IDE utilizada com os pacotes de extensão Jupyter e Python.

## **Clonar o Repositório do Projeto**

Abra seu terminal ou prompt de comando e clone o repositório para sua máquina local através do comando:

```bash
git clone https://github.com/BruninSouza/relatorios_auditoria_interna_governamental.git
```



## **Instalação das dependencias do projeto**

Primeiro crie um ambiente virtual para evitar conflitos de dependências com o comando:

```bash
  python3 -m venv venv
```

ative o ambiente virtual:

* Linux/macOS
```bash
  source venv/bin/activate
```

* Windows
```bash
  .\venv\Scripts\activate
```

Após ativar o ambiente virtual, instale as bibliotecas necesárias para o projeto:

```bash
  pip install --upgrade pip
  pip install -r requirements.txt
```
