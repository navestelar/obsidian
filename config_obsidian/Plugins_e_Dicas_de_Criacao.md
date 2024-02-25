<br><br>
# Plugins 

<br>

### Diagrams.net
- **Função ->** Criar diagramas e UMLs.
- **Como usar ->** Dentro do arquivo clicar *botão direito* e depois em *insert new diagram*
- **Dica ->** A cor do obsidian é #1E1E1E então se quiser criar um objeto minimalista pode utilizar essa cor e branco nas linhas. Existe um diagrams normal sem o .net que faz isso automaticamente, mas bugou no meu PC (Felipe) e não funcionou mais.


<br><br>

### Advanced Tables

- **Função ->** Formatar tabelas markdown.
- **Como usar ->** Ao digitar o titulo ele já formata, mas fica assim:

	```
	| Titulo 1 | Titulo 2 |
	| -------- | -------- |
	| Dado 1   | Dado 2   |   
	```

<br><br>

### HTML Tag Autocomplete
- **Função ->** Completar tags;
- **Como usar ->** Só digitar a TAG e ele completa o final;

<br><br>

### Markdown Formatting Assistant
- **Função ->** Facilita o uso de tags Markdown e HTML com um menu bem completo de funções
- **Como usar ->** No canto superior direito tem um simbolo de expandir e nas opções tem o HTML e Markdown.

<br><br>

### Code Emitter

- **Função ->** Dentro de bloco de códigos é possível executar códigos menores para testar seu funcionamento
- **Como usar ->** Qualquer código escrito pode ser executável dentro do bloco de código. Ex:

```java
public class Main {
	public static void main(String[] args){
		System.out.println("Testando Main");
	}
}
```


<br><br>

# Dicas de criação 

São necessárias dicas de criação pois no momento de alteração futura desse repositório para outro sistema de arquivos pode dar conflito com carácteres desconhecidos.

<br><br>

**Nomes de arquivos ->** Os nomes de arquivos devem ser compostos por **underline ( _ )** no lugar do espaço e não devem conter caracteres de acentuação e nem caracteres especiais;

**Nomes das pastas ->** Devem ser compostos somente por letras minusculas e também utilizar **underline ( _ )** no lugar dos espaços e não devem conter caracteres de acentuação e nem caracteres especiais;

**Criação do Glossário ->** Sempre que criar uma pasta no obsidian tambem crie um arquivo com o nome da pasta assim pode ter um ponto de acesso através de links dos arquivos nas pastas anteriores. Por exemplo o arquivo README.md acessa a pasta faculdade através do link do arquivo Faculdade.md;

**Forma de criação dos Links ->** Sempre que criar um link dentro de um arquivo use a forma abaixo e sempre coloque o (.md) no final do arquivo, assim os links podem ser acessados no obsidian através do glossário e tambem no GitHub para pesquisa online.

```Markdown
[Nome de apresentacao do link](pasta_de_acesso/Arquivo_a_Ser_Acessado.md)
```


