#faculdade 

## Introdução 

<div style="text-align: Justify">Uma transação é qualquer ação que lê ou grava em um banco de dados. Ela pode consistir de um simples comando <strong>SELECT</strong> que gere uma lista de conteúdo da tabela, de uma serie de comandos <strong>UPDATE</strong> relacionados que alterem os valores de atributos em diferentes tabelas, de diversos comandos <strong>INSERT</strong> que adicionem linhas a uma ou mais tabelas ou de uma combinação desses três tipos de comandos.

<br>

A maioria das transações são formadas por duas ou mais solicitações. A <strong>A solicitação de banco de dados</strong> é o equivalente a um único comando de SQL em um aplicativo ou transação. Por exemplo se uma transação for composta por dois comandos <strong>UPDATE</strong> e um comando <strong>INSERT</strong>, ela deve utilizar três solicitações de banco de dados. 

</div>


<br><br>

<div style="text-align: Justify">Um exemplo que mostra bem como funciona as transações é a transferência de valores entre contas correntes, que é uma operação unica do ponto de vista do cliente, porém dentro do banco de dados essa transferência envolve várias operações como: 

<br>
<strong>1 - Verificar o saldo da sua conta</strong>
<br>
<strong>2 - Tirar o valor da sua conta</strong>
<br>
<strong>3 - Colocar o valor na conta de outra pessoa</strong>
</div>

<br><br>

## ACID 

<div style="text-align: Justify"><strong>ACID</strong> é a sigla para as características principais que definem como devem ser feitas transações: <strong>Atomicidade, Consistência, Isolamento e Durabilidade</strong></div>


<br>

#### Atomicidade / Indivisibilidade

<div style="text-align: Justify">Cada instrução de uma transação (leitura, gravação, atualização ou exclusão de dados) é tratada como uma única unidade. Ou as instruções são todas executadas ou nenhuma é executada. Essa propriedade evita perda ou corrupção de dados.</div>

<br>

#### Consistência

<div style="text-align: Justify">Garante que as transações apenas modifiquem as tabelas de maneiras predefinidas e previsíveis. A consistência transacional mantém as tabelas consistentes em caso de corrupção de dados ou erros, evitando resultados de execução não intencionais.</div>

<br>

#### Isolamento

<div style="text-align: Justify">Vários usuários podem ler e gravar na mesma tabela ao mesmo tempo, mas as transações são isoladas para que as simultâneas não interfiram ou afetem umas às outras. Na verdade, cada solicitação é tratada como se estivesse ocorrendo de forma independente, mesmo que ocorram simultaneamente.</div>

<br>

#### Durabilidade

<div style="text-align: Justify">Garante que as alterações de dados feitas por transações executadas com sucesso sejam preservadas, mesmo em caso de falha do sistema.</div>


<br><br>

## Comandos 

Comando para desligar os commits automáticos assim sempre que dermos um <strong>INSERT</strong> os dados não serão gravados até um <strong>COMMIT</strong> ser executado. Na sequencia tem um comando para verificar o status do autocommit. 

```sql
SET @@autocommit = OFF;
SELECT @@autocommit;
```


<br><br>

## Base para Testes

<br><br>

## Recuperação de Transações

- As transações são salvas na tabela de LOG mesmo depois de um ROLLBACK?
- Como funciona o LOG de transações do MySQL?

<br>

**Existem dois algorítimos de recuperação que são:**
- **UNO/NO-REDO**
- **UNO/REDO**


