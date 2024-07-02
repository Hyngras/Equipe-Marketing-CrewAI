# AI Developer Marketing Project

Este projeto utiliza a framework CrewAI para criar e gerenciar uma equipe de agentes autônomos que ajudam na criação de estratégias de marketing digital. Os agentes são capazes de analisar concorrentes, desenvolver campanhas de marketing e gerar conteúdos criativos. O projeto também integra uma interface com o WhatsApp para interação direta com os usuários.

## Estrutura do Projeto

- `main.py`: Script principal para inicializar agentes e tarefas, criar equipes e processar informações.
- `whatsapp.py`: Script para integrar a funcionalidade principal do projeto com o WhatsApp, permitindo interação direta via mensagens.
- `agents.py`: Define os agentes utilizados no projeto, incluindo seus papéis, objetivos e ferramentas.
- `tasks.py`: Define as tarefas que os agentes devem executar, detalhando suas descrições e resultados esperados.
- `drive.py`: Funções auxiliares para autenticação e interação com o Google Drive para extração de textos.
- `requirements.txt`: Lista de dependências do projeto.

## Funcionalidades

1. **Análise de Produto**: Analisa o site do produto fornecido pelo usuário para identificar recursos, benefícios e pontos de venda únicos.
2. **Análise de Concorrentes**: Identifica e analisa os principais concorrentes do produto, fornecendo uma comparação detalhada.
3. **Desenvolvimento de Campanha**: Cria estratégias de marketing detalhadas e ideias de conteúdo criativo para campanhas de mídia social.
4. **Geração de Conteúdo**: Gera cópias de anúncios envolventes para Instagram.
5. **Fotografia e Revisão**: Descreve e revisa opções de fotografia para postagens no Instagram.

## Configuração

### Pré-requisitos

- Python 3.8 ou superior
- Ambiente virtual (recomendado)

### Instalação

1. Clone este repositório:

    ```bash
    git clone https://github.com/seu-usuario/AI-developer-Marketing.git
    cd AI-developer-Marketing
    ```

2. Crie e ative um ambiente virtual:

    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows use `venv\Scripts\activate`
    ```

3. Instale as dependências:

    ```bash
    pip install -r requirements.txt
    ```

4. Configure as variáveis de ambiente:

    Crie um arquivo `.env` na raiz do projeto e adicione as seguintes variáveis:

    ```env
    GROQ_API_KEY=your_groq_api_key
    SERPER_API_KEY=your_serper_api_key
    WHATSAPP_ACCESS_TOKEN=your_whatsapp_access_token
    WHATSAPP_PHONE_NUMBER_ID=your_whatsapp_phone_number_id
    ```

5. Configure as credenciais do Google Drive:

    Baixe suas credenciais JSON do Google Cloud Console e salve como `credentials.json` na raiz do projeto.

### Execução

1. Execute o script principal:

    ```bash
    python main.py
    ```

2. Para iniciar a integração com o WhatsApp:

    ```bash
    python whatsapp.py
    ```

## Uso

Após iniciar o script `whatsapp.py`, você pode interagir com os agentes enviando mensagens para o número configurado no WhatsApp. Os agentes responderão com análises detalhadas, estratégias de marketing e conteúdo gerado.

## Estrutura do Código

### `main.py`

- Inicializa os agentes e tarefas.
- Cria equipes de cópia e imagem.
- Processa informações fornecidas pelo usuário.

### `whatsapp.py`

- Configura a API do WhatsApp Business.
- Processa mensagens recebidas e envia respostas geradas pelos agentes.

### `agents.py`

Define os agentes:

- `analista_mercado`
- `estrategista_marketing`
- `especialista_criativo`
- `especialista_fotografia`
- `diretor_criativo`

### `tasks.py`

Define as tarefas:

- `analise_produto`
- `analise_concorrente`
- `campanha_desenvolvimento`
- `copia_instagram`
- `captura_fotografia`
- `revisao_foto`

### `drive.py`

- Funções para autenticação e interação com o Google Drive.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
