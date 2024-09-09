# POO - Desafio de Modelagem e Diagramação do Componente iPhone

## Descrição do Desafio

Neste desafio, você será responsável por modelar e diagramar a representação **UML** do componente **iPhone**, abrangendo suas funcionalidades principais como:

- **Reprodutor Musical**
- **Aparelho Telefônico**
- **Navegador na Internet**

### Contexto

Com base no vídeo de lançamento do iPhone de **2007**, especificamente entre os minutos **00:15 e 00:55**, você deve elaborar um **diagrama UML** que represente as funcionalidades descritas a seguir. Em seguida, é opcional implementar as classes e interfaces no formato de arquivos **.java**.

#### Funcionalidades a Modelar

1. **Reprodutor Musical**
    - `tocar()`: Inicia a reprodução de uma música.
    - `pausar()`: Pausa a reprodução atual.
    - `selecionarMusica(String musica)`: Seleciona uma nova música para tocar.

2. **Aparelho Telefônico**
    - `ligar(String numero)`: Realiza uma chamada para o número especificado.
    - `atender()`: Atende uma chamada recebida.
    - `iniciarCorreioVoz()`: Inicia o correio de voz.

3. **Navegador na Internet**
    - `exibirPagina(String url)`: Exibe a página da web correspondente ao URL fornecido.
    - `adicionarNovaAba()`: Abre uma nova aba no navegador.
    - `atualizarPagina()`: Atualiza a página da web atual.

### Objetivo

- Criar um **diagrama UML** que represente as funcionalidades descritas acima.
- Implementar as classes e interfaces correspondentes em **Java** (opcional).

### Diagrama UML

```mermaid
classDiagram
    class iPhone {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }
    class AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }
    class NavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet