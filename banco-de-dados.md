# Banco de Dados

## Banco de Dados escolhido

Inicialmente no projeto enquanto monolito, o tempo havia escolhido o MySQL como banco de dados para o projeto, mas quando houve uma migração para a nuvem suportada pela AWS Services, o MySQL foi substituído pelo Amazon Aurora MySQL, e agora com a implementação dos microsserviços optamos para usar o MongoDB que será usado na nuvem através do Amazon DocumentDB que é compatível com o MongoDB.

Essa decisão nos permitiu aproveitar as vantagens de se ter um banco de dados não relacionado, orientado a documentos, mais flexível, adequado ao ambiente de nuvem e fazendo com que a refatoração fosse a menor dentre os outros microsserviços.

Os motivos da escolha pelo MongoDB / Amazon DocumentDB estão detalhados abaixo, ressaltando que o termo MongoDB será utilizado para se referir a ambos, exceto na subseção que descreve a substituição do MySQL pelo Amazon DocumentDB.

### SGDB Não Relacional

Ao contrário do MySQL, o MongoDB não exige um esquema rígido predefinido. Isso significa que você pode adicionar campos aos documentos conforme necessário, proporcionando uma maior agilidade no desenvolvimento e evitando a necessidade de alterar esquemas existentes.

Para operações que envolvem leituras intensivas, o MongoDB pode oferecer desempenho superior, especialmente em consultas que aproveitam a estrutura de documentos aninhados sem a necessidade de juntas complicadas.

### Custo

O MongoDB oferece uma versão gratuita em nuvem através do MongoDB Atlas, o que condiz com o objetivo educacional do projeto.

### Substituição do MySQL pelo MongoDB/DocumentDB

Durante a transição do projeto de monolito para microsserviços e sua migração para a nuvem AWS, o MySQL foi inicialmente substituído pelo Amazon Aurora MySQL. No entanto, a escolha estratégica mais recente recaiu sobre o MongoDB, integrado ao Amazon DocumentDB.

Essa mudança permitiu flexibilidade no esquema, agilizando o desenvolvimento e evitando alterações frequentes nos esquemas existentes. Além disso, o MongoDB proporcionou desempenho superior em leituras intensivas, especialmente em consultas com documentos aninhados, simplificando operações sem a necessidade de junções complexas. Essa adaptação  não só manteve a coerência na nuvem, mas também contribuiu para a eficiência operacional e custos, com a oferta gratuita do MongoDB Atlas para fins educacionais no âmbito do projeto.

## Collection

### Pagamento

![fast-n-foodious-data-model.png](diagramas/fast-n-foodious-data-model.png)
