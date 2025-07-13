# [DIO](www.dio.me) - Trilha Java Básico

## Autores
- [Gleyson Sampaio](https://github.com/glysns)

## POO - Desafio

### Modelagem e Diagramação de um Componente iPhone

Neste desafio, você será responsável por modelar e diagramar a representação UML do componente iPhone, abrangendo suas funcionalidades como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

### Diagrama UML (Mermaid)

```mermaid
classDiagram
    class iPhone

    class ReprodutorMusical {
        - String musicaAtual
        - boolean estaTocando
        - List~String~ playlist
        - int volume
        + tocar()
        + pausar()
        + proximaMusica()
        + musicaAnterior()
        + selecionarMusica(String musica)
    }

    class AparelhoTelefonico {
        - String numeroAtual
        - boolean emChamada
        - List~String~ historicoChamadas
        - boolean correioVozAtivo
        + ligar(String numero)
        + atender()
        + iniciarCorreioVoz()
    }

    class NavegadorInternet {
        - String urlAtual
        - List~String~ abas
        - int abaAtual
        - boolean paginaCarregando
        + exibirPagina(String url)
        + adicionarNovaAba()
        + atualizarPagina()
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet

````

### Instruções
1. Assista ao vídeo do lançamento do iPhone para entender as funcionalidades principais.
2. Utilize uma ferramenta UML de sua preferência para criar o diagrama das classes e interfaces. Você pode utilizar o modelo acima (criado na sintaxe [Mermaid](https://mermaid.js.org/)), uma alternativa open-source e compatível com arquivos Markdown como este.
3. Opcionalmente, caso esteja cheio(a) de confiança, pode implementar as classes Java representadas em seu diagrama UML.
4. Submeta seu repositório GitHub conforme as orientações da plataforma DIO. Por exemplo:

```bash
https://github.com/glysns/trilha-java-basico/desafios/poo/README.md
```` 
