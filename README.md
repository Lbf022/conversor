# 📄 Conversor de Moedas em Java

Este projeto é um conversor de moedas simples desenvolvido em **Java**, utilizando uma **API de câmbio online** para obter as taxas de conversão em tempo real. A aplicação roda no console e oferece um menu interativo para o usuário escolher diferentes conversões entre moedas da América Latina e o Dólar Americano.

## 🚀 Funcionalidades

- Conversão entre:
  - Dólar Americano ↔ Peso Argentino
  - Dólar Americano ↔ Real Brasileiro
  - Dólar Americano ↔ Peso Colombiano
- Exibição das taxas de câmbio para as moedas:
  - ARS (Peso Argentino)
  - BOB (Boliviano)
  - BRL (Real Brasileiro)
  - CLP (Peso Chileno)
  - COP (Peso Colombiano)
  - USD (Dólar Americano)
- Interface via menu no console
- Atualização em tempo real via **ExchangeRate API**

## 🛠️ Tecnologias utilizadas

- Java 11+
- `HttpClient` (requisições HTTP)
- `Gson` (para processar JSON)
- [ExchangeRate API](https://www.exchangerate-api.com/)

## 📦 Dependências

Você precisa adicionar a biblioteca [**Gson**](https://github.com/google/gson) ao seu projeto.

Se estiver usando um gerenciador de dependências como Maven, adicione ao `pom.xml`:

```xml
<dependency>
  <groupId>com.google.code.gson</groupId>
  <artifactId>gson</artifactId>
  <version>2.10.1</version>
</dependency>
```

Ou, se estiver compilando manualmente, baixe o `.jar` do Gson e inclua no classpath.

## 📋 Como usar

1. **Clone ou copie** o repositório.
2. **Abra o projeto em sua IDE** Java favorita (Eclipse, IntelliJ, VS Code...).
3. **Adicione a biblioteca Gson**.
4. Substitua a variável `chave` pelo **seu token da ExchangeRate API**:
   ```java
   String chave = "SUA_CHAVE_AQUI";
   ```
5. Compile e execute o projeto.
6. Use o menu interativo no console para converter moedas ou visualizar as taxas.

## 🧪 Exemplo de uso

```
=== CONVERSOR DE MOEDAS ===
1 - Dólar Americano → Peso Argentino
2 - Peso Argentino → Dólar Americano
3 - Dólar Americano → Real Brasileiro
4 - Real Brasileiro → Dólar Americano
5 - Dólar Americano → Peso Colombiano
6 - Peso Colombiano → Dólar Americano
7 - Exibir taxas filtradas (ARS, BOB, BRL, CLP, COP, USD)
0 - Sair
Escolha uma opção: 3
Digite o valor em Dólar Americano: 100
100.00 Dólar Americano = 525.00 Real Brasileiro
```

## 📌 Observações

- A precisão das conversões depende da resposta da API.
- O programa exige conexão com a internet.
- O número de requisições gratuitas da API pode ser limitado dependendo do plano.

## 🧑‍💻 Autor

**Lucas Bandeira Ferreira**  
Projeto desenvolvido para fins acadêmicos e práticos de aprendizado em Java com integração de APIs.
