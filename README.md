# Projeto albums — Java Web com HttpServer

## Atividade
- Exercício da disciplina de SPOLBP2
- Entregue no ultimo bimestre de 2026

## Estrutura
- `src/org/ifspspo/Main.java`: servidor HTTP, leitura do CSV, filtros SSR e API JSON.
- `albuns.csv`: arquivo fornecido na atividade; mantenha-o na raiz do projeto.

## Requisitos
- JDK 11 ou superior.
- Não utiliza bibliotecas externas.

## Como executar
Na raiz do projeto, basta compilar:

```bash
javac --add-modules jdk.httpserver -encoding UTF-8 -d out src/org/ifspspo/Main.java
```

Execute:

```bash
java --add-modules jdk.httpserver -cp out org.ifspspo.Main
```

Mantenha o terminal aberto enquanto testa o servidor.

## Rotas
- http://localhost:8080/albuns — todos os álbuns (SSR).
- http://localhost:8080/2026 — álbuns lançados em 2026 (SSR).
- http://localhost:8080/pop — álbuns do gênero Pop (SSR).
- http://localhost:8080/api/albuns — todos os álbuns em JSON (API/CSR).

Essa aplicação espera encontrar `albuns.csv` no diretório de execução (raiz do projeto).
O arquivo CSV original não está incluído no ZIP para evitar substituir ou alterar o arquivo fornecido pelo professor.
