# API Explorer

**API Explorer** é uma ferramenta para explorar e verificar os endpoints disponíveis em uma API RESTful. O script realiza requisições a uma lista pré-definida de endpoints usando diferentes métodos HTTP e registra os resultados em um arquivo `routes.txt`.

## Funcionalidades

- Verifica automaticamente os endpoints especificados.
- Suporte a múltiplos métodos HTTP (`GET`, `POST`, `PUT`, `DELETE`).
- Substituição dinâmica de parâmetros como `{id}` com valores de teste.
- Armazena as rotas disponíveis em um arquivo de texto.

## Requisitos

- Python 3.6 ou superior
- Biblioteca `requests`

## Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/devGabyAlves/api-explorer.git
   cd api-explorer

2. Crie um ambiente virtual (opcional, mas recomendado):
    python -m venv venv
    source venv/bin/activate  

3. Instale as dependências necessárias:
    pip install requests

## Como Usar

1. Edite o arquivo api_explorer.py para definir o base_url e, se necessário, adicionar ou remover endpoints na lista endpoints.

2. Execute o script:
    python api_explorer.py

3. O resultado da verificação será salvo no arquivo routes.txt.

## Exemplo de Saída

GET - https://api.exemplo.com/users
POST - https://api.exemplo.com/users/register
GET - https://api.exemplo.com/products/1
PUT - https://api.exemplo.com/orders/10/status

## Exemplo de Saída

- Adição de Novos Endpoints: Edite a lista de endpoints no arquivo api_explorer.py para incluir novos caminhos a serem verificados.
- Métodos HTTP: Por padrão, o script verifica GET, POST, PUT e DELETE. Você pode adicionar ou remover métodos alterando a lista methods dentro da função check_endpoints.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.
1. Faça um fork do repositório.
2. Crie uma branch para sua modificação (git checkout -b feature/modificacao).
3. Commit suas alterações (git commit -m 'Adiciona nova funcionalidade').
4. Faça o push para a branch (git push origin feature/modificacao).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a MIT License.

## Contato

Para dúvidas ou sugestões, entre em contato com gabriellysthefany.alves@gmail.com
