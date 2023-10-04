# Desafio de Código 01 - Formação C++

Este é o projeto do Desafio de Código 01 da Formação C++. Neste projeto, estamos construindo um sistema bancário simples que incorpora os conceitos de Programação Orientada a Objetos (POO) e Programação Orientada a Aspectos (AOP) usando a linguagem Java e a extensão AspectJ.

## Objetivo

O objetivo deste projeto é demonstrar como podemos aplicar o Paradigma de Programação Orientado a Aspectos (AOP) para adicionar funcionalidades de verificação de saldo em um sistema bancário. Vamos criar uma função transversal que verifica o saldo antes de permitir saques em diferentes contas bancárias.

## Estrutura do Projeto

- **`src/`**: Contém o código-fonte Java do projeto principal.
  - `ContaBancaria.java`: Implementa as classes de conta bancária.
  - `SistemaBancario.java`: Implementa o programa principal.
- **`aspect/`**: Contém o código-fonte AspectJ para a verificação de saldo.
  - `VerificacaoSaldoAspect.java`: Implementa o Aspecto para a verificação de saldo.
- **`lib/`**: Pode conter as bibliotecas do AspectJ, se necessário.
- **`aop.xml`**: Arquivo de configuração do AspectJ.
- **`README.md`**: Este arquivo de documentação.

## Pré-requisitos

- Eclipse IDE com o plugin AJDT (AspectJ Development Tools) instalado.
- Java Development Kit (JDK) instalado.
- Configurações de ambiente do AspectJ configuradas corretamente.

## Como Executar o Projeto

1. Clone este repositório para o seu ambiente de desenvolvimento local.

2. Abra o Eclipse IDE.

3. Importe o projeto:
   - No Eclipse, vá para "File" (Arquivo) -> "Import" (Importar).
   - Escolha "General" (Geral) -> "Existing Projects into Workspace" (Projetos Existente no Espaço de Trabalho).
   - Selecione o diretório onde você clonou este repositório como o diretório raiz do projeto.

4. Configure o AspectJ no projeto:
   - Clique com o botão direito do mouse no projeto e vá para "Properties" (Propriedades).
   - No menu à esquerda, clique em "AspectJ" (ou "AspectJ Compiler").
   - Marque a caixa "Enable project specific settings" (Habilitar configurações específicas do projeto) e configure as opções de acordo com as necessidades.

5. Execute o projeto:
   - Clique com o botão direito do mouse no arquivo `SistemaBancario.java` no pacote `src`.
   - Selecione "Run as Java Application" para iniciar o programa.

6. O AspectJ aplicará automaticamente o Aspecto `VerificacaoSaldoAspect` antes de qualquer chamada ao método `sacar` em uma instância de `ContaBancaria`, verificando o saldo antes do saque.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas (issues) e solicitar melhorias (pull requests).

## Licença

Este projeto está sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para obter detalhes.

