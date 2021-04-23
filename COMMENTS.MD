# Documentação

url api https://apigrupoa.herokuapp.com/api/

url admin https://georgetassiano-grupoa.netlify.app/

usuario: admin@admin.com
senha: password

## API Laravel

# pacotes utilizados
laravel/sanctum  - pacote responsável por fornecer autenticação por token para API

laravellegends/pt-br-validator - pacote responsável por fornecer validações de requisições que só existem no brasil, como cpf, cnpj, etc.

owen-it/laravel-auditing - pacote responsável por gerar log automático de ações dos usuários do sistema logado.

prettus/l5-repository - pacote responsável por gerir a camada de repositories com o banco de dados, e assim oferecendo usos apropriados com o Eloquent, DB, entre outros.

laracasts/generators - pacote responsável por gerar um pequeno gerador de migrations e outros arquivos internos do laravel, utilizando somente linha de comando.

lucascudo/laravel-pt-br-localization - pacote responsável por fornecer a internacionalização brasileira de respostas automáticas do laravel de tudo que ele já fornece automaticamente, como por exemplo erros de validações de requests.


#camadas da aplicação
 Middlewares -> Requests/Resources <-> Controllers <-> Services <-> Repositories 

 A camada de serviços é composta por classes responsáveis pela regra de negócio a ser executada, chamando se necessário um ou mais repositories para buscar/atualizar/criar/excluir dados na base de dados e retornando para o controller que o chamou com a resposta da requisição. 
 
# O que ainda faltaria ser adicionado
utilização do pacote "spatie/laravel-permission" que junto com o Guard do Laravel realiza toda a questão de roles e permissions do sistema, associado a cada um usuário.

HTTP tests, Browsers Tests, Testes de integração e de Banco de Dados. 

Tratamento de exceções  em toda a aplicação com o disparo de e-mail para os administradores do sistema.

Validação de 2 fatores dos usuários do sistema.


## Admin Nuxt.js

# pacotes utilizados
@nuxtjs/auth-next  - pacote responsável por fornecer autenticação por token com API

"@nuxtjs/axios"- pacote responsável por fornecer client http para requisições

"@nuxtjs/pwa"- pacote responsável fornencer a pwa da aplicação do front 

"nuxt" - Framework Server-Side renderer para Vue, mais confiável, estável e utilizado pela comunidade, para aplicações de dashboard que podem escalar com alto desempenho.

"@nuxtjs/vuetify" - biblioteca de UI Kit com melhores apis de components altamente adaptaveis e robustos.


# O que ainda faltaria ser adicionado
utilização do pacote "vee-validate" para validar todo campo de input que existe no admin

HTTP tests, Browsers Tests, Testes de integração e Testes unitários.

Tratamento de exceções  em toda a aplicação com o disparo de e-mail para os administradores do sistema.

Validação de 2 fatores dos usuários do sistema.

campo de pesquisa só filtra o que está já está na página atual, e não no servidor.

bug de paginação quando seleciona carregar todos os dados, pois existe mais páginas a serem navegadas e que não existem dados nelas. 

design system  do admin, com documentação completa feito no figma e / ou  zeplin.io 

página inicial do dashboard contendo alguns contadores , mostrando por exemplo quantos alunos existem no sistema.

crud de gerir os usuários administrativos do sistema

crud de definir os grupos e permissões dos usuários administrativos do sistema

crud de logs de ações dos usuários administrativos.

