# 📚 LiterAlura

Aplicação em **Java + Spring Boot** que consome a API de livros do Projeto Gutenberg e permite pesquisar, salvar e consultar livros e autores em um banco de dados.

A aplicação roda no **terminal (CLI)** e foi desenvolvida como parte do **Challenge LiterAlura (Alura + Oracle ONE)**.

---

# 📌 Funcionalidades

- 🔎 Buscar livros pelo título via API
- 📖 Listar livros registrados no banco de dados
- ✍️ Listar autores registrados
- 📅 Listar autores vivos em determinado ano
- 🌎 Listar livros por idioma
- 💾 Persistência de dados com JPA

---

# 🖥️ Menu da Aplicação

```
*********************************
*          LITERALURA           *
*********************************

1 - Buscar livro pelo título
2 - Listar livros registrados
3 - Listar autores registrados
4 - Listar autores vivos em determinado ano
5 - Listar livros por idioma
0 - Sair

Escolha uma opção válida:
```

---

# 🧱 Estrutura do Projeto

```
desafio-literalura
│
├── src
│   └── main
│       └── java
│           └── br.com.literalura
│               ├── principal
│               │   └── Principal.java
│               │
│               ├── model
│               │   ├── Livro.java
│               │   └── Autor.java
│               │
│               ├── repository
│               │   ├── LivroRepository.java
│               │   └── AutorRepository.java
│               │
│               └── service
│                   └── ConsumoAPI.java
│
└── resources
    └── application.properties
```

---

# 🔗 API Utilizada

API pública:

https://gutendex.com

Dados disponíveis:

- título
- autores
- idiomas
- número de downloads

---

# ⚙️ Tecnologias

- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- Maven
- PostgreSQL
- IntelliJ IDEA

---

# ▶️ Como Executar

## 1️⃣ Clonar repositório

```bash
git clone https://github.com/seu-usuario/desafio-literalura.git
```

## 2️⃣ Configurar banco

Editar:

```
src/main/resources/application.properties
```

Exemplo:

```
spring.datasource.url=jdbc:postgresql://localhost/literalura
spring.datasource.username=usuario
spring.datasource.password=senha
```

## 3️⃣ Rodar projeto

Via Maven:

```bash
mvn spring-boot:run
```

Ou execute a classe `Principal.java` pela IDE.

---

# 📚 Objetivo

Praticar:

- consumo de APIs REST
- manipulação de JSON
- persistência de dados com JPA
- arquitetura em camadas
- desenvolvimento backend com Spring Boot

---

# 👨‍💻 Autor

Desenvolvido por **Vitor Beltrão**