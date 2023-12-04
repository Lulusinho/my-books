
<h1 align = center> Resumo do <a href=https://github.com/brunocampos01/banco-de-dados/blob/master/livros/Sistemas%20de%20Banco%20de%20Dados%20navathe%206%C2%AA%20Edicao.pdf>livro</a> de BD </h1>

- Banco de dados é uma coleção de dados, onde dados são fatos que tem significado

---

- **Definir** envolve especificar os tipos, estrutura e restrição dos dados 

- **Metadados** armazena informações sobre os dados para melhor catalogo.
- **Construção** é o processo de armazenar dados através da SGBD
- **Manipulação** consulta, atualização e geração de relatórios sobre os dados
- **Compartilhamento** para que diversos usuários possam acessá-lo 

<img src = img1.png width = 400px/>
<font size = 2%> os retangulos são software e abstrações enquanto os cilindros são objetos físicos como armazenamentos</font>

---
A redundância no banco de dados gera ineficiência e desperdício de espaço.

### Natureza de autodescrição de um sistema
- O sistema contém uma descrição completa da estrutura e restrições. Esse catalogo é usado pelo SGBD.
- O catalogo armazena os metadados que especifica e descreve cada tabela. Assim o SGBD utiliza-o para saber o que fazer com os dados.
- Dessa forma é possível criar um  único SGBD para usar diversos banco de dados. Pois ele usará o catálogo para cada banco de dados.

### Isolamento entre programa e dados, e abstração de dados
**Independência** de dados do programa é quando a estrutura dos dados é alterado e os programas de acesso não tenham que ser alterado da mesma forma, pois existe uma separação através do SGDB.

##### Abstração de dados
- É quando existe uma independência entre os dados e as operações. Isso é oferecido através do SGBD através de representações conceituais dos dados. Dessa forma não é necessário se preocupar com detalhes dos dados.

### View 
- Diferentes usuários exigem diferentes visões, é um subconjunto do banco de dados ou dados virtuais

### Compartilhamento e processamento de multiusúarios

Para um sistema que suporte vários é necessário que o SGBD use controle de concorrência, para garantia da confiabilidade dos dados. Ex: OLPT (Online Transaction Processing)
#### Propriedades
- Isolamento: Faz com que cada transação pareça que execute de forma isolada
- Atomicidade: Se uma é executada, todas serão

