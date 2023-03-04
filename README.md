# :construction: README customizado em construção ! :construction:
<!-- Olá, Tryber!
Esse é apenas um arquivo inicial para o README do seu projeto no qual você pode customizar e reutilizar todas as vezes que for executar o trybe-publisher.

Para deixá-lo com a sua cara, basta alterar o seguinte arquivo da sua máquina: ~/.student-repo-publisher/custom/_NEW_README.md

É essencial que você preencha esse documento por conta própria, ok?
Não deixe de usar nossas dicas de escrita de README de projetos, e deixe sua criatividade brilhar!
:warning: IMPORTANTE: você precisa deixar nítido:
- quais arquivos/pastas foram desenvolvidos por você; 
- quais arquivos/pastas foram desenvolvidos por outra pessoa estudante;
- quais arquivos/pastas foram desenvolvidos pela Trybe.
-->

# Projeto mysql-all-for-one

- início:
  - Foi realizado no projeto da Trybe, com o codinome All For One em que praticamos todos os conceitos de SQL que foi ensinados; Porém, utilizamos um  banco de dados totalmente diferente, então dê tchau para o sakila e dê boas vindas ao Northwind, que é um banco de dados de uma empresa fictícia que vende produtos para restaurantes.
---
## Habilidades:

* Temos, nesse projeto, uma série de desafios com diferentes níveis de complexidade que devem ser resolvidos cada um em seu próprio arquivo.

* Leia a pergunta e chore na raiz do projeto um arquivo chamado desafioN.sql, em que N é o número do desafio;

* O arquivo deve conter apenas o código SQL do desafio resolvido. Não se esqueça de incluir o ponto e vírgula (";") no final de suas consultas e também de colocar o nome do banco_de_dados.tabela_por_completo , como no exemplo a seguir:

* SELECT * FROM northwind.orders;
Faça isso até finalizar todos os desafios.

* Para entregar o seu projeto, você deve criar um repositório Pull Request neste. Este Pull Request deve conter os arquivos desafio1.sql, desafio2.sqle assim por diante o desafio27.sql, que conterão até seu código SQLde cada desafio, respectivamente.

* Não é necessário colocar USE northwind ou SET SQL_SAFE_UPDATES = 0;no início dos seus arquivos.

- Após a execução dos testes locais, o banco de dados northwindé deletado.

- aviso É importante que seus arquivos tenham exatamente estes nomes!aviso
Você pode adicionar outros arquivos se necessário. Qualquer dúvida, procure uma monitoria.

* Lembre-se de que você pode consultar nosso conteúdo sobre Git & GitHub e nosso Blog - Git & GitHub sempre que precisar!

- espiral_calendárioDados de Entrega
- Orientações
- baleiaRodando no Docker vs Localmente
---
### - Com Docker;
avisoAntes de começar, seu docker-compose precisa estar na versão 1.29 ou superior.Veja aqui ou na documentação como instalá-lo. No primeiro artigo, você pode substituir onde está com 1.26.0por 1.29.2.

 - fonte de informaçãoRode os serviços nodee dbcom o comando docker-compose up -d.

 - Lembre-se de parar o mysqlse estiver usando localmente na porta padrão ( 3306), ou adapte, caso queria fazer uso da aplicação em containers
 - Esses serviços irão inicializar um container chamado all_for_onee outro chamado all_for_one_db.
 - A partir daqui você pode rodar o container all_for_onevia CLI ou abri-lo no VS Code.
fonte de informaçãoUse o comando docker exec -it all_for_one bash.

 - Ele te dará acesso ao terminal interativo do container criado pelo compose, que está rodando em segundo plano.
 - As credenciais de acesso ao banco de dados estão definidas no arquivo docker-compose.yml, e são acessíveis no container através das variáveis ​​de ambiente MYSQL_USERe MYSQL_PASSWORD.lâmpada
fonte de informaçãoInstale as dependências [ Caso existam ] comnpm install . (Instale dentro do container)

- avisoAtenção: Caso opte por utilizar o Docker, TODOS os comandos disponíveis no package.json(npm start, npm test, npm run dev, ...) devem ser executados DENTRO do container, ou seja, no terminal que aparece após a execução do comando docker execcitado acima .

 - avisoAtenção: O git dentro do container não vem configurado com suas credenciais. Ou faça os commits fora do container, ou configure como suas credenciais do git dentro do container.

 - avisoAtenção: Não rode o comando npm audit fix! Ele atualiza várias dependências do projeto, e essa atualização gera conflitos com o avaliador.

 - brilhos Dica: A extensão Remote - Containers(que estará na seção de extensões recomendadas do VS Code) é indicada para que você possa desenvolver sua aplicação no container Docker direto no VS Code, como você faz com seus arquivos locais.

* teste de sequela

---
### - Sem Docker;
 - fonte de informaçãoRode o comando npm startpara iniciar o servidor em modo de desenvolvimento.

 - fonte de informaçãoRode o comando npm testpara executar os testes.

 - fonte de informaçãoRode o comando npm run devpara iniciar o servidor em modo de desenvolvimento com nodemon.

 - fonte de informaçãoInstale as dependências [ Caso existam ] comnpm install

 - avisoAtenção: Não rode o comando npm audit fix! Ele atualiza várias dependências do projeto, e essa atualização gera conflitos com o avaliador.

 - brilhosDica: Para rodar o projeto desta forma, obrigatoriamente você deve ter o nodeinstalado em seu computador.

 - brilhosDica: O avaliador espera que a versão do nodeutilizada seja a 16.

---
