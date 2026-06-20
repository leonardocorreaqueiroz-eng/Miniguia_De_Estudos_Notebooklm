# # README – Caderno Temático: Boas Práticas de Linguagem e Estruturação de Código em Java

## 1. Contexto e Objetivos

### Tema Escolhido

O tema escolhido para este caderno temático foi **Boas Práticas de Linguagem e Estruturação de Código em Java**.

A escolha desse tema ocorreu devido à sua importância para o desenvolvimento de software profissional. Durante o aprendizado da linguagem Java, percebe-se que escrever código funcional não é suficiente; é necessário desenvolver soluções legíveis, organizadas, reutilizáveis e fáceis de manter.

### Objetivos de Estudo

Os principais objetivos deste estudo foram:

* Compreender as convenções de nomenclatura da linguagem Java.
* Aprender os fundamentos da Orientação a Objetos aplicados à organização do código.
* Entender princípios de desenvolvimento como SOLID e DRY.
* Identificar práticas que aumentam a qualidade e a manutenibilidade do software.
* Conhecer ferramentas e processos utilizados no mercado para desenvolvimento profissional.
* Criar um material de consulta para futuras revisões e aplicação em projetos pessoais.

---

# 2. Curadoria de Fontes

As seguintes fontes abertas foram selecionadas e utilizadas como base para as consultas realizadas no NotebookLM:

## 1. Cubos Academy

**Tema:** Boas práticas e padrões de código em Java

Link:
https://blog.cubos.academy/java-boas-praticas-e-padroes-de-codigo/

### Contribuição para o estudo

* Convenções de nomenclatura
* Clean Code
* Organização de projetos
* Boas práticas de desenvolvimento

---

## 2. DevMedia

**Tema:** História e evolução da tecnologia Java

Link:
https://www.devmedia.com.br/a-historia-da-tecnologia-java-easy-java-magazine-1/18446

### Contribuição para o estudo

* Evolução da linguagem
* Contexto histórico
* Consolidação do Java no mercado

---

## 3. Repositório UFPB – Gateway Project

**Tema:** Exemplo prático de projeto Java

Link:
https://github.com/zaqueumoura/Gateway-Project

### Contribuição para o estudo

* Estruturação de pacotes
* Organização de classes
* Aplicação prática da Orientação a Objetos

---

## 4. DIO

**Tema:** História e evolução da linguagem Java

Link:
https://www.dio.me/articles/a-historia-e-evolucao-linguagem-programacao-java-3ac053f644eb

### Contribuição para o estudo

* Evolução da linguagem
* Recursos modernos
* Aplicações atuais do Java

---

# 3. Engenharia de Prompts e "Cicatrizes"

Esta seção documenta o processo utilizado para obter respostas mais relevantes da IA, demonstrando as tentativas, dificuldades e refinamentos realizados.

## Prompt Inicial

### Pergunta

> De acordo com as fontes enviadas, me diga que tipo de boas práticas eu devo ter desde o início com a linguagem e estruturação do código.

### Resultado Obtido

A IA apresentou recomendações relacionadas a:

* Convenções de nomenclatura
* Orientação a Objetos
* Encapsulamento
* Interfaces
* SOLID
* DRY
* Tratamento de exceções
* Testes automatizados
* Git
* IDEs modernas

### Dificuldade Encontrada

A resposta foi abrangente, porém muito geral, sem exemplos concretos de aplicação.

### Aprendizado

Perguntas muito amplas geram respostas mais genéricas.

---

## Prompt Refinado 1

### Pergunta

> Quais práticas um desenvolvedor Java júnior deve aplicar em seus primeiros projetos para evitar código difícil de manter?

### Resultado Obtido

A IA destacou:

* Responsabilidade Única (SRP)
* Encapsulamento
* Separação de responsabilidades
* Nomenclatura adequada
* Evitar duplicação de código

### Aprendizado

Especificar o perfil do desenvolvedor tornou a resposta mais objetiva e prática.

---

## Prompt Refinado 2

### Pergunta

> Gere exemplos de código Java demonstrando boas e más práticas de nomenclatura, encapsulamento e tratamento de exceções.

### Resultado Obtido

A IA forneceu exemplos comparativos mostrando:

* Nomes inadequados versus nomes descritivos
* Uso correto de atributos privados
* Tratamento adequado de exceções

### Aprendizado

Solicitar exemplos de código facilita a compreensão dos conceitos teóricos.

---

## Prompt Refinado 3

### Pergunta

> Organize todas as boas práticas encontradas nas fontes em um guia de estudos para um estudante de Java.

### Resultado Obtido

Foi gerado um material estruturado contendo:

* Conceitos fundamentais
* Boas práticas
* Ferramentas recomendadas
* Organização lógica para revisão

### Aprendizado

Prompts voltados para organização de conteúdo ajudam a transformar informações dispersas em material de estudo.

---

## Principais Dificuldades (Troubleshooting)

| Problema                  | Solução                                  |
| ------------------------- | ---------------------------------------- |
| Respostas muito genéricas | Tornar a pergunta mais específica        |
| Falta de exemplos         | Solicitar exemplos de código             |
| Excesso de teoria         | Pedir aplicações práticas                |
| Conteúdo disperso         | Solicitar organização em formato de guia |

---

# 4. Miniguia de Estudo (Entrega Final)

## 4.1 Resumo Estruturado

### Convenções de Nomenclatura

Seguir as convenções oficiais do Java melhora a legibilidade e facilita a colaboração entre desenvolvedores.

#### Padrões recomendados

**Classes e Interfaces**

```java
public class ProcessadorPagamento
```

**Métodos e Variáveis**

```java
double calcularTotal()
```

**Constantes**

```java
public static final int MAX_CLIENTES = 100;
```

---

### Orientação a Objetos

A Orientação a Objetos é a base da estruturação de aplicações Java.

#### Conceitos fundamentais

* Encapsulamento
* Herança
* Polimorfismo
* Abstração

#### Exemplo de Encapsulamento

```java
public class Conta {

    private double saldo;

    public double getSaldo() {
        return saldo;
    }

    public void depositar(double valor) {
        saldo += valor;
    }
}
```

---

### Princípios SOLID

SOLID é um conjunto de princípios que auxiliam na construção de software flexível e fácil de manter.

#### Benefícios

* Menor acoplamento
* Maior reutilização
* Facilidade de manutenção
* Melhor testabilidade

---

### Princípio DRY

DRY significa:

> Don't Repeat Yourself

Evite duplicar lógica de negócio.

Quando identificar códigos repetidos, crie métodos ou classes reutilizáveis.

---

### Tratamento de Exceções

Boas práticas:

* Nunca deixar blocos `catch` vazios.
* Utilizar exceções específicas.
* Utilizar `try-with-resources` quando necessário.

Exemplo:

```java
try (BufferedReader br = new BufferedReader(new FileReader("arquivo.txt"))) {
    System.out.println(br.readLine());
}
```

---

### Testes Automatizados

Testes ajudam a garantir que novas alterações não quebrem funcionalidades existentes.

Ferramentas comuns:

* JUnit
* Mockito

Benefícios:

* Maior confiabilidade
* Facilidade para refatoração
* Menor quantidade de bugs

---

### Ferramentas Importantes

#### Controle de Versão

Git deve ser utilizado desde os primeiros projetos.

Benefícios:

* Histórico de alterações
* Trabalho colaborativo
* Recuperação de versões anteriores

#### IDEs

Ferramentas recomendadas:

* IntelliJ IDEA
* Eclipse
* NetBeans

#### Análise de Código

Ferramentas úteis:

* SonarQube
* Checkstyle

---

# 4.2 Glossário

| Conceito       | Definição                                                          |
| -------------- | ------------------------------------------------------------------ |
| SOLID          | Conjunto de princípios para desenvolvimento orientado a objetos    |
| SRP            | Uma classe deve possuir apenas uma responsabilidade                |
| DRY            | Evitar duplicação de código                                        |
| Clean Code     | Práticas para tornar o código legível e sustentável                |
| Encapsulamento | Proteção dos dados internos da classe                              |
| Interface      | Contrato que define comportamentos                                 |
| Herança        | Reutilização baseada em especialização                             |
| Composição     | Reutilização baseada em relacionamento entre objetos               |
| Optional       | Classe utilizada para representar valores que podem estar ausentes |
| Git            | Sistema de controle de versão                                      |
| JUnit          | Framework para testes unitários                                    |
| Mockito        | Framework para criação de objetos simulados em testes              |
| IDE            | Ambiente Integrado de Desenvolvimento                              |

---

# 4.3 Prompts Reutilizáveis para Revisão

## Explicação de Conceitos

> Explique este conceito Java utilizando exemplos simples e analogias do mundo real.

---

## Comparação de Boas Práticas

> Compare boa prática e má prática para este trecho de código Java.

---

## Refatoração

> Refatore este código seguindo os princípios SOLID e Clean Code.

---

## Resumo de Conteúdo

> Crie um resumo estruturado deste assunto utilizando apenas as fontes fornecidas.

---

## Questões de Revisão

> Gere 10 questões de revisão com gabarito comentado sobre este conteúdo.

---

## Plano de Estudos

> Monte um plano de estudos de 7 dias para dominar este tema.

---

# Conclusão

O estudo demonstrou que escrever código profissional vai além de fazer o programa funcionar. A adoção de convenções de nomenclatura, princípios de Orientação a Objetos, SOLID, DRY, testes automatizados e ferramentas de versionamento contribui diretamente para a qualidade, manutenção e evolução do software. Além disso, o uso estratégico de prompts permitiu extrair respostas mais úteis e organizadas da IA, transformando informações dispersas em um material estruturado de aprendizado.
