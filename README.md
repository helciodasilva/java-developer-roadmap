# Java Developer Roadmap
- [ ] Docker
    - [X] Dockerfile
    - [X] Docker Compose
    - [ ] Kubernates
    - [ ] Docker Swarm

- [ ] Monolitos
    - [ ] Um único projeto
    - [ ] Vantagens:
        - [ ] Não precisa ser escalável
        - [ ] Projetos mais simples
        - [ ] Facilidade para codificar
    - [ ] Desvantagens:
        - [ ] Dificuldade para escalar
        - [ ] Gastos com máquina (por ter que duplicar o servidor e escalar o sistema inteiro)
        - [ ] Dificuldade de dar manutenção

- [ ] Microservices

    - [ ] Conceito:
        - [ ] Serviços independentes
        - [ ] Bancos separados
        - [ ] Se comunicam entre si
        - [ ] Automação da infraestrutura
        - [ ] Tolerante a falha: desenhado para falhar

    - [ ] Vantagens:
        - [ ] Tem um único propósito
        - [ ] Facilidade para escalar

    - [ ] Desvantagens:
        - [ ] Sistema/infraestrutura mais complexo
        - [ ] Transferimos toda a complexidade da construção do sistema para a infraestrutura
        - [ ] O time precisa ter uma boa cultura de codificação
        - [ ] O time prática cultura de testes
        - [ ] a Equipe precisa dominar DDD
        - [ ] O time deve conhecer a arquitetura de software
        - [ ] Conhecimento de banco nosql
        - [ ] cultura devops
        - [ ] Orquestração e comunicação
        - [ ] Monitoramente e resolução de falhas
        - [ ] O projeto realmente precisa ser microserviços?

- [ ] Testes automatizados
    - [X] Unidade
    - [X] Teste de Regressão
    - [ ] Integração
    - [ ] Aceitação
    - [ ] TDD
    - [ ] BDD
    - [ ] Frameworks
        - Java
            - [X] JUnit
            - [ ] Mockito
            - [ ] webclient Spring
            - [ ] mockserver
            - [X] Selenium

- [ ] AWS
    - [X] Amazon S3
        - [X] Bucket
        - [X] Site estático
    - [ ] Amazon Lambda
- [ ] Mensageria
    - [ ] Mensagem X Evento
    - [ ] Consumer
    - [ ] Producer
    - [ ] Dead letter queue
      - [ ] In message queueing the dead letter queue is a service implementation to store messages that meet one or more of the following criteria:
        - [ ] Message that is sent to a queue that does not exist.
        - [ ] Queue length limit exceeded.
        - [ ] Message length limit exceeded.
        - [ ] Message is rejected by another queue exchange.
        - [ ] Message reaches a threshold read counter number, because it is not consumed. Sometimes this is called a "back out queue".

- [X] API RESTFull
    - [X] Versionamento da API (header, uri)
    - [X] Não utilizar verbos de ação no mapeamento
    - [X] Utilizar os métodos corretamente (GET, POST, PUT, DELETE, PATCH)
    - [X] Utilizar o status de resposta corretamente
    - [X] Não utilizar verbos no path
    - [X] HATEOS (Hypermidia)
    - [X] Separar palavras com hífen (user-service)
    - [X] Não definir no path representação do recurso (clentes.json, clientes.xml)
    - [X] Não abreviar palavras
    - [X] Não utilizar barra (/) no final
    - [X] Declarar recurso no plural (users)

- [X] Documentação de APIs (Swagger, Spring REST Docs)

- [ ] Design Pattern
    - [ ] Criação
        - [X] Singleton
        - [ ] Factory Method
        - [ ] Builder
    - [ ] Comportamental
        - [X] Strategy
        - [ ] Observer
    - [ ] Facade
- [ ] Stack Spring
    - [ ] Spring Framework
        - [ ] Injeção de dependências
        - [X] Beans
        - [X] Cache
        - [X] Paginação
        - [X] Job scheduler
        - [X] CORS
        - [X] Validações com Bean Validation
        - [X] Profiles
        - [X] Interceptors
        - [X] AOP

    - [ ] Spring Boot
    - [ ] Spring Data
        - [X] Repositórios
        - [X] Transações
        - [X] Lazy Loading
        - [ ] Spring Data REST
    - [X] Actuator
    - [X] Spring Boot Admin
    - [X] Exception Handler
    - [ ] Spring Reativo

- [ ] Spring Cloud: Framework utilizado para a criação de microservices
    - [ ] Config-repo
    - [ ] Eureka
    - [ ] API Gateway
        - [ ] Zuul Service
        - [ ] Gateway Service
    - [ ] Feign Client
    - [ ] Bulkhead: Histrix
    - [ ] Fallback: Circuit Breaker
    - [ ] Sleuth
- [ ] Java:
    - [X] 5
        - [X] Generics
        - [X] Enhanced For
        - [X] Enumerations
        - [X] Autoboxing e unboxing
    - [X] 7:
        - [X] Pacote NIO
        - [X] Executors
        - [X] Inferência na Criação de Objetos de Tipos Genéricos (Diamont Operator)
        - [X] Separador de dígitos em literais numéricos (5_000 e 5_000.0)
        - [X] Variáveis do tipo String em comandos switch
        - [X] varargs
        - [X] Multicatch

    - [ ] 8:
        - [ ] Streams
            - [ ] Collectors
            - [ ] Comparator
            - [ ] Filter
            - [ ] Map e FlatMap
            - [ ] Distinct
            - [ ] Sorted
            - [ ] Reduce
        - [ ] Optional
        - [ ] API de Datas
        - [ ] Interface Funcional (Consumer, Predicate, Supplier). Possui apenas um método
        - [ ] Lambda Expression
        - [ ] Method Reference
        - [ ] Default Methods
    - [ ] 9
        - [ ] Modularização (Java Plataform Module System)
        - [ ] Factory Method
        - [ ] JShell
        - [ ] Melhorias no Garbage Collector G1
        - [ ] Http Client 2
        - [ ] Fluxos reativos
    - [ ] 10
        - [ ] Alteração no versionamento do java
        - [ ] Inferência de tipos para variáveis locais (var)
    - [X] 11
        - [X] Single File Source Code
        - [X] Preview Feature
    - [ ] 12

    - [ ] 13
        - [ ] Preview Feature
            - [ ] Text block
            - [ ] Switch Expressions
            - [ ] Text Blocks
    - [ ] 12
        - [ ] Complete Feature
            - [ ] Switch Expressions
        - [ ] Preview
            - [ ] Pattern Matching for instanceof
            - [ ] Text Blocks
            - [ ] Helpful NullPointerExceptions
            - [ ] Records 
- [ ] SOLID

    - [ ] Single Responsibility Principle: 
        - [ ] Uma classe deve ter apenas uma responsabilidade
        - [ ] Problemas por falta de coesão:
            - [ ] Alto acoplamento
            - [ ] Dificuldade de implementar testes
            - [ ] Dificuldade de reaproveitar código

    - [ ] Open–closed Principle
        - [ ] Abertos para extensão
        - [ ] Fechados para modificação
        - [ ] Extender e não modificar

    - [ ] Liskov Substitution Principle

    - [ ] Interface Segregation Principle
        - [ ] Não forçar uma classe a implementar interfaces que não vai usar
        - [ ] Evitar interfaces genéricas

    - [ ] Dependency Inversion Principle
        - [ ] Devemos depender de abstrações e não implementações

- [ ] Clean Code
    - [ ] São ténicas ou uma filosofia para desenvovlimento de software
    - [ ] Criado por Uncle Bob

    - [ ] Princípios

        - [ ] Definições de nomes
            - [ ] O nome precisa passar uma ideia central
            - [ ] Não tem problema o nome ser grande
            - Padrão adotado:
                - [ ] Nome de verbos e funções: verbos (escrever())
                - [ ] Classes e objetos: substantivos (caneta) 

        - [ ] Regra do escoteiro: Deixar o código mais limpo do que estava antes de editá-lo
            
        - [ ] Criar testes automatizados antes de fazer alguma mudança no código

        - [ ] Estruturar bem o código
            - [ ] Funções devem ser pequenas
            - [ ] Devem executar apenas uma tarefas. Facilitando a manutenção e reutilização do código

        - [ ] DRY Don't repeat yourself
            - [ ] Não duplicar código

        - [ ] Código bem escrito é muito melhor que um comentários
            - [ ] Comentar somente o necessário
            - [ ] O código deverá ser revisado junto com o código

        - [ ]  Tratar corretamente as exceções 

- [ ] Segurança:
    - [ ] Enumeração de senha
    - [ ] Brute force
    - [ ] DDoS
    - [ ] WAF
    - [ ] IDS, IPS
    - [ ] Rate limit
    - [ ] Vulnerabilidades
    - [ ] SSL/HTTPS
    - [ ] Criptografia assimétrica e simétrica
- [X] Frameworks
    - [X] Lombok
    - [X] ModelMapper
    - [X] Quarkus
- [X] git e gitflow
- [X] nginx
    - [X] Proxy Reverso
    - [X] Load Balance
    - [X] CDN
- [X] Integração contínua
    - [X] Gitlab CI
    - [X] Jenkins
    - [X] Sonar
- [X] Boas práticas
    - [X] Code Review

- [X] Bancos
    - [X] MySQL
    - [X] Oracle
    - [X] SQL Server
    - [X] MongoDB

- [X] Servidores
    - [X] Tomcat
    - [X] JBoss
    - [X] Wildfly
    
- [X] Build:
    - [X] Semantic Version
    - [X] Maven
    - [X] Gradle

## Teste de software

Escrever um [teste automatizado][1] não é tarefa tão árdua. Ele, na verdade, se parece muito com um teste manual. Imagine um desenvolvedor que deva testar o comportamento do carrinho de compras da loja virtual quando existem dois produtos lá cadastrados: primeiramente, ele “clicaria em comprar em dois produtos”, em seguida “iria para o carrinho de compras”, e por fim, verificaria “a quantidade de itens no carrinho (deve ser 2)” e o “o valor total do carrinho (que deve ser a soma dos dois produtos adicionados anteriormente)”.

Ou seja, de forma generalizada, o desenvolvedor primeiro pensa em um cenário (dois produtos comprados), depois executa uma ação (vai ao carrinho de compras), e por fim, valida a saída (vê a quantidade de itens e o valor total do carrinho).

Um [teste automatizado][1] é similar. Ele descreve um cenário, executa uma ação e valida uma saída. A diferença é que quem fará tudo isso será a máquina, sem qualquer intervenção humana.

[Testes automatizados][1] são fundamentais para um desenvolvimento de qualidade, e é obrigação de todo desenvolvedor escrevê-los. Sua existência traz diversos benefícios para o software, como o aumento da qualidade e a diminuição de bugs em produção.

### Teste de Unidade

Um [teste de unidade][1] não se preocupa com todo o sistema; ele está interessado apenas em saber se uma pequena parte do sistema funciona.

Um [teste de unidade][1] testa uma única unidade do nosso sistema. Geralmente, em sistemas orientados a objetos, essa unidade é a classe. A ideia é termos baterias de testes de unidade separadas para cada uma dessas classes; cada bateria preocupada apenas com a sua classe.

## Teste de Regressão

Se algum dia um outro desenvolvedor alterar esse código, ele poderá executar a bateria de testes automatizados existente e descobrir se a sua alteração fez alguma funcionalidade que já funcionava anteriormente parar de funcionar. Isso é conhecido como [testes de regressão][1]. Eles garantem que o sistema não regrediu.

### Frameworks

#### JUnit

É o framework de testes de unidade mais popular do mundo Java

## Java

### Java 5

#### Import Estático
```diff
-import org.junit.Assert;
+import static org.junit.Assert.assertEquals;
import org.junit.Test;

import br.com.helciodasilva.commons-util.conversor.Converter;

public class ConverterTest {

  @Test
  public void shouldConverter() {
    Converter converter = new Converter();
    int number = converter.converte("I");
-   Assert.assertEquals(1, numero);
+   assertEquals(1, number);
  }

}
```

### Java 8

#### Stream

##### Snippets
```java
// flatMap de List<Map<K,V>>
Map<K, V> map = values.stream() //
    .map(service::retrieveVMap) // Map<K,V>
    .flatMap(m -> m.entrySet().stream()) //
    .collect(Collectors.toMap(Map.Entry::getKey, Map.Entry::getValue, (p1, p2) -> p1));
```

### Java 9

#### Convenience Factory Methods for Collections (JEP 269)
- Simplifica a criação de Coleções e Mapas
- Retorna um objeto mutável
- Não permite chaves e valores nulos (NullPointerException)
- Set e Map não permitem valores duplicados (IllegalArgumentException)

```diff
-List<String> list = new ArrayList<>();
-list.add("Java");
-list.add("Kotlin");
-list = Collections.unmodifiableCollection(list);
+List<String> list = List.of("Java","Kotlin");  

-Set<String> set = new HashSet<>();
-set.add("Java");
-set.add("Kotlin");
-Collections.unmodifiableCollection(set);
+Set<String> set = Set.of("Java","Kotlin");  

-HashMap<Integer, String> map = new HashMap<>();
-map.put(1, "Java");
-map.put(2, "Kotlin");
-Collections.unmodifiableMap(map);
+Map<Integer, String> map = Map.of(1, "Java", 2, "Kotlin");

-Map.Entry<Integer, String> entry = new AbstractMap.SimpleEntry<>(1, "Java");
+Map.Entry<Integer, String> entry = Map.entry(1, "Java");

-HashMap<Integer, String> map = new HashMap<>();
-map.put(entry.getKey(), entry.getValue());
+Map<Integer, String> map = Map.ofEntries(entry);  
```

Por que foram criados 11 extra métodos e não utilizaram var-args?
```diff
-static <E> List<E> of(E... e1) {
+static <E> List<E> of(E e1) {
  return new ImmutableCollections.List12<>(e1);
}
-static <E> List<E> of(E e1, E e2) {
- return new ImmutableCollections.List12<>(e1, e2);
-}
```
Performance. Com var-args teria a criação desnecessária de objetos

#### jshell (JEP 222)
O [jshell][2] é uma nova ferramenta de linha de comando do JDK nada mais é do que um ambiente interativo, extremamente amigável, no qual você pode executar códigos Java e receber feedback imediato. Esse conceito é conhecido como REPL (Read-Eval-Print-Loop), e existe desde o tempo do LISP, lá pelos anos 60. Ele também é bastante usado em linguagens como Scala, Clojure, Haskell e Ruby.

```bash
# Iniciando o JShell
jshell

# Comando para onde por onde começar
/help intro

# Fechando o JShell
/exit

# Executando um comando incompleto
/exi

# Declarando variáveis de forma implícita
"Java"
$5 ==> "Java"

# Utilizando uma variável criada de forma implícita
$5.toUpperCase()

# Listando todos os snippets usados
/list

# Desabilitando o feedback de declarações e execução de expressões com retorno
/set feedback silent
$5 ==> "Java"

# Desabilitando o feedback em modo verboso
/set feedback verbose

# Editando um snippet
/list
/edit 4

# Definindo o vim como editor padrão
/set editor vim

# Apagando um snippet
/list
/drop 4

# Importando uma classe
import java.util.stream.*;
import static java.util.stream.Stream.of;

# Listando imports
/imports

# Importando uma classe automaticamente (Shift + tab + i)
LocalDate
0: Do nothing
1: import: java.time.LocalDate

# Assign to local variable (Shift + Tab v)
new UserDTO()
UserDTO _ = new UserDTO()

# Utilizando o autocomplete (Tab)
Str
String

# Visualizando o javadoc de um método (Precinar Tab apóes a abertura dos parênteses)
"java".lenght(

# Carregando um arquivo com a seção do JShell ativa
open arquivo

# Carregando um arquivo carregando uma nova seção do JShell
jshell arquivo

```
##### Atalhos
| Atalho | Descrição                             |
|--------|---------------------------------------|
| Ctrl+a | Moveocursorparaoiníciodalinha         |
| Ctrl+e | Moveocursorparaofinaldalinha          |
| Alt+b  | Voltaumapalavra                       |
| Alt+f  | Avançaumapalavra                      |
| Ctrl+r | Buscaporcomandosouinstruçõesdigitados |

##### Comandos
| Comando  | Descrição                                                           |
|----------|---------------------------------------------------------------------|
| /reload  | Para limpar sua seção do JShell                                     |
| /save    | nome-doarquivo Para salvar todos os snippets da seção atual         |
| /open    | nome-doarquivo Para abrir o jShell com todos os snippets salvos     |
| /open    | Para importar a declaração dessa classe existente AlgumaClasse.java |
| /history | Para mostrar seu histórico de comandos executados na seção          |

## Java 11

### Preview Feature (JEP 12)

Uma [preview feature][4] é uma funcionalidade implementada, mas ainda não é padrão na JDK e é necessário habilitar o compilador para podermos usá-la: javac --enable-preview --release. Um outro ponto importante, é que por ser uma preview feature, existe a possibilidade de ser atualizada ou até mesmo removida nas próximas versões do Java.

### Launch Single-File Source-Code Programs (JEP 330)

O [código-fonte de arquivo][3] único permite que executemos programas diretamente da fonte.

A JVM compila o arquivo de origem na memória e, em seguida, executa o primeiro método público main() que encontrar.

Formas de ativar a executação de arquivo:
- O primeiro item na linha de comandos seguido pelas opções da JVM é um nome de arquivo com a extensão .java
- A linha de comandos contém a opção --source

### Arquivos com extensão .java
```java
public class HelloWorld {

  public static void main(String[] args) {
    System.out.println("Hello World");
  }
}
```
```diff
-javac HelloWorld.java
-java HelloWorld
+java HelloWorld.java
```

### Arquivos Shebang
É comum em sistemas derivados do Unix, como macOS e Linux, usar o "#!" diretiva para executar um arquivo de script executável.

Conteúdo do arquivo hello
```java
#!/opt/java --source version
public class HelloWorld {

  public static void main(String[] args) {
    System.out.println("Hello World");
  }
}
```

```bash
# Tornando o arquivo executável
chmod +x hello

# Executando um arquivo como um script
./hello
/home/dev/hello # Informando o path completo

# Utilizando explicitamente o iniciador para chamar o arquivo shebang:
java --source 11 hello # A opção --source é necessária mesmo se já estiver presente no arquivo. O shebang no arquivo é ignorado e é tratado como um arquivo java normal sem a extensão .java.
```

## Java 14

### (Preview Feature) Records (JEP 359)
Um record é um tipo de classe que serve para representar dados
```diff
-@Data
-public class User {
+public record User (@NotBlank String name, @NotBlank String login, boolean admin) {
-
- @NotBlank 
- private String name;
-
- @NotBlank 
- private String login;
-
-
- private boolean admin;
-
}
```

```diff
-public class UserDTO {
+public record UserDTO(String name, String login, String mail) {
- private final String name;
- private final String login;
- private final String mail;
-
- public UserDTO(String name, String login, String mail) {
-   this.name = name;
-   this.login = login;
-   this.mail = mail;
- }
-
- public String getName() {
-   return name;
- }
-
- public String getLogin() {
-   return login;
- }
-
- public String getMail() {
-   return mail;
- }
-
- @Override
- public int hashCode() {
-   final int prime = 31;
-   int result = 1;
-   result = prime * result + ((login == null) ? 0 : login.hashCode());
-   result = prime * result + ((mail == null) ? 0 : mail.hashCode());
-   result = prime * result + ((name == null) ? 0 : name.hashCode());
-   return result;
- }
-
- @Override
- public boolean equals(Object obj) {
-   if (this == obj)
-     return true;
-   if (obj == null)
-     return false;
-   if (getClass() != obj.getClass())
-     return false;
-   UserDTO other = (UserDTO) obj;
-   if (login == null) {
-     if (other.login != null)
-       return false;
-   } else if (!login.equals(other.login))
-     return false;
-   if (mail == null) {
-     if (other.mail != null)
-        return false;
-   } else if (!mail.equals(other.mail))
-     return false;
-   if (name == null) {
-     if (other.name != null)
-       return false;
-   } else if (!name.equals(other.name))
-     return false;
-   return true;
- }
-
- @Override
- public String toString() {
-   return "UserDTO [name=" + name + ", login=" + login + ", mail=" + mail + "]";
- }
-
}
```
```diff
public class UserService {

  public User create(User user) {
-     if (user.isAdmin()) {
+     if (user.admin()) {
      }
  }

}
```

```java
@RestController
@RequestMapping("v1/users")
public class UserRestController {

  @Autowired
  private UserService userService;

  @GetMapping
  public Collection<UserDTO> find(UserQuery userQuery){
      Collection<UserDTO> payload = userService.find(userQuery);
      return ResponseEntity.ok(payload);
  }

  @ResponseStatus(HttpStatus.CREATED)
  @PostMapping
  public UserDTO create(@RequestBody User user) {
      Collection<UserDTO> payload = userService.create(user);
      return ResponseEntity.ok(payload);
  }

}
```

## Spring Cloud

### Circuit Breaker

É uma implementação Circuit Breaker para trabalhar com tolerância a falhas

#### Config
pom.xml
```diff
<parent>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-parent</artifactId>
  <version>2.3.2.RELEASE</version>
  <relativePath/> <!-- lookup parent from repository -->
</parent>

<properties>
  <java.version>1.8</java.version>
+ <spring-cloud.version>Hoxton.M3</spring-cloud.version>
</properties>

<dependencies>
+ <dependency>
+   <groupId>org.springframework.cloud</groupId>
+   <artifactId>spring-cloud-starter-netflix-hystrix</artifactId>
+ </dependency>
< dependencies>

+<dependencyManagement>
+ <dependencies>
+   <dependency>
+     <groupId>org.springframework.cloud</groupId>
+     <artifactId>spring-cloud-dependencies</artifactId>
+     <version>${spring-cloud.version}</version>
+     <type>pom</type>
+     <scope>import</scope>
+   </dependency>
+ </dependencies>
+</dependencyManagement>
```

## git

```bash
# Alterando o conteúdo de arquivos de um commit
git commit --amend --no-edit
```

## Microservices

### gateway
O que é um [gateway][7]?
O o Gateway é uma interface que recebe as chamadas para seus sistemas internos, sendo uma grande porta de entrada. 

Ele pode atuar de cinco diferentes maneiras:
- Filtro para o tráfego de chamadas;
- Única porta de entrada para as diversas APIs;
- Componente essencial do gerenciamento de APIs;
- Roteador do tráfego nas APIs e de Rate Limit;
- Mecanismo de segurança, com autenticação e log.

### Tolerância a falhas

A [Tolerância a falhas][6] é a propriedade que permite que sistemas continuem a operar adequadamente mesmo após as falhas em alguns de seus componentes.

A meta para tudo que devemos projetar em torno de tolerância de falha é minimizar a intervenção humana. Implementar rotinas de falha automática tem que ser parte de cada chamada de serviço que está acontecendo

## Mensagaria

### Stream Events

[Stream Events][5] é um pouco diferente de uma fila simples. Stream Events garante que se escalarmos o sistema que lê a fila, a informação irá chegar em apenas um sistema.

## Design Patterns

### Creational Design Patterns 

#### Singleton
Garante que uma classe tenha apenas uma instância mantendo um ponto global de acesso à ela

Lazy Initialization
```java
public class UserService {

  private static UserService instance;

  private UserService() { // Private constructor private to make sure that there is no other way to instantiate the class
  }
  public static UserService getInstance() {
      if (instance == null) {
        instance = new UserService(); //  creates a new instance of the class if one does not exist
      }
      return instance; // If an instance has already been created, the constructor simply returns a reference to that object.
  }
}
```

Eager initialization:
```java
public class UserService {
  // Always creates an instance
  private static final UserService INSTANCE = new UserService(); // the final keyword here enables the class to actually be a singleton, i.e. ensures that only one instance exists
 
  private UserService() {}
 
  public static UserService getInstance() {
    return INSTANCE;
  }
}
```

#### Factory Method

- Encapsula o processo de criação de objetos
- Fornece uma interface para criar um objeto, mas permite às subclasses decidirem qual tipo de objeto instanciar
- A complexidade de criação de um objeto fica em uma outra classe, que não será a classe que está utilizando o método.
- Facilita a manutenção porque o código fica isolado em um único lugar

Objetos são criados através de uma interface (interface ou classe absrata)
As classes concreatas criará o objeto em tempo de execução.

Um Factory Method é um método que cria e retorna novos objetos. Uma fábrica é uma classe que contém um ou mais métodos de fábrica.

Exemplos de implementações:
- DriverManager.getConnection(databaseName, username, password);
- Class.forName("com.mysql.jdbc.Driver");
- clazz.newInstance();
- integer.valueOf();
- Calendar.getInstance()
- ResourceBundle.getBundle()
- NumberFormat.getInstance()
- Charset.forName()

```java
public interface Moeda {
  String getSimbolo();
}

class Real implements Moeda {
  @Override
  public String getSimbolo() {
    return "R$";
  }
}

class USDolar implements Moeda {
  @Override
  public String getSimbolo() {
    return "USD";
  }
}
```
```java
public enum Pais {
  BRASIL, EUA;
}
```
```java
public class MoedaFactory {
  public static Moeda createMoeda(Pais pais) {
    switch (pais) {
    case BRASIL:
      return new Real();
    case EUA:
      return new Real();
    default:
      throw new IllegalArgumentException("Nao existe esse pais");
    }
  }
}
```
```diff
-Moeda moeda = new Real();
+Moeda moeda = MoedaFactory.createMoeda(Pais.BRASIL);
```

## kotlin
kotlin é uma linguagem de programação:
- Pragmática que combina os paradigmas de Orientação a Objetos e Programação Funcional
- com foco em interoperabilidade, segurança, clareza e suporte a ferramentas
- tem total interoperabilidade com Java, ou seja, podemos utilizar códigos que foram  escritos em Java no nosso código em Kotlin	
- é uma linguagem mais concisa (menos verbosa) comparada à Java
- não possui tipos primitivos

Compilador online: https://try.kotlinlang.org

```diff
-public class Principal {
- public static void main(String[] args) {
- }
-}
+fun main(args: Array<String>) {
+}

// Single-line Comments

/*
Multi-line Comments
*/

-System.out.println("Hello World");
+println("Hello World")

-@Data
-public class User {
-
- private String name;
- private String email;
-
-}
+data class User(var name: String, var email: String)

-String username = "";
+var username :String = ""
-username.length();
+username.length

-String username = null;
+var username :String? = null;
-username.length();
+username?.length

// Sempre defina como val. Use var somente se precisar alterar o valor
-final var username = "helcioasilva";
+val username = "helciodasilva"

final Integer count = 100;
val	count: Int = 100

-var count = 1_000_000
+var count = 1_000_000

var username = "helciodasilva"
-var message = String.format("username: %s", username);
+var message = "username> $username"

var message = """
	Hello
	World
-	""";
+	"""

-int[] values = {1, 2, 3, 4};
+var values :Array<Int> = arrayOf(1, 2, 3, 4)
-var value = values[0]
+var value = values[0];

-List<Integer> values = new ArrayList<>();
-values.add(1);
-values.add(2);
+val values = mutableListOf(1,2)

-List<Integer> values = List.of(1, 2);
+val value = listOf(1,2)

+var value = values.stream().filter(v -> v % 2 == 0).collect(Collectors.toList);
+val value = values.filter{it % 2 == 0 }
```

### Estruturais
### Comportamentais


## Sourcetree

### Configurand o WinMerge como External Diff Tool
```bash
Tools ->
	Options ->

		Diff ->

			# x64
				External Diff Tool: Custom
				Diff Command: C:\Program Files\WinMerge\WinMergeU.exe
				Arguments: -u -e $LOCAL $REMOTE
		
				Merge Diff Tool: Custom
				Diff Command: C:\Program Files\WinMerge\WinMergeU.exe
				Arguments: -u -e -dl \"Local\" -dr \"Remote\" $LOCAL $REMOTE $MERGED

			# x86		
				External Diff Tool: Custom
				Diff Command: C:\Program Files (x86)\WinMerge\WinMergeU.exe
				Arguments: -u -e $LOCAL $REMOTE
		
				Merge Diff Tool: Custom
				Diff Command: C:\Program Files (x86)\WinMerge\WinMergeU.exe
				Arguments: -u -e -dl \"Local\" -dr \"Remote\" $LOCAL $REMOTE $MERGED
```

[1]: https://www.casadocodigo.com.br/products/livro-tdd
[2]: https://www.casadocodigo.com.br/products/livro-java9
[3]: https://www.codeflow.site/pt/article/java-single-file-source-code
[4]: https://www.infoq.com/br/articles/records-no-java-14
[5]: https://www.udemy.com/course/comunicacao-entre-microservices-usando-spring-cloud/learn/lecture/16288988#overview
[6]: https://www.udemy.com/course/comunicacao-entre-microservices-usando-spring-cloud/learn/lecture/16289176#overview
[7]: https://www.udemy.com/course/comunicacao-entre-microservices-usando-spring-cloud/learn/lecture/16291808#overview