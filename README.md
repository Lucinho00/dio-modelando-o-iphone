# dio-modelando-o-iphone

1. Diagrama UML
Vamos criar o diagrama UML para representar as funcionalidades do iPhone como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

Diagrama UML
+-----------------------+
|      ReprodutorMusical|
+-----------------------+
| +tocar(): void        |
| +pausar(): void       |
| +selecionarMusica(musica: String): void |
+-----------------------+

+-----------------------+
|     AparelhoTelefonico|
+-----------------------+
| +ligar(numero: String): void  |
| +atender(): void       |
| +iniciarCorreioVoz(): void |
+-----------------------+

+-----------------------+
|   NavegadorNaInternet |
+-----------------------+
| +exibirPagina(url: String): void |
| +adicionarNovaAba(): void        |
| +atualizarPagina(): void         |
+-----------------------+

+-----------------------+
|        iPhone         |
+-----------------------+
| +tocar(): void        |
| +pausar(): void       |
| +selecionarMusica(musica: String): void |
| +ligar(numero: String): void  |
| +atender(): void       |
| +iniciarCorreioVoz(): void |
| +exibirPagina(url: String): void |
| +adicionarNovaAba(): void |
| +atualizarPagina(): void  |
+-----------------------+
2. Implementação em Java
Interface ReprodutorMusical
public interface ReprodutorMusical {
    void tocar();
    void pausar();
    void selecionarMusica(String musica);
}
Interface AparelhoTelefonico
public interface AparelhoTelefonico {
    void ligar(String numero);
    void atender();
    void iniciarCorreioVoz();
}

Passos para Resolver o Desafio
Criar o Diagrama UML

Identificar as classes e interfaces necessárias.
Definir os métodos de cada interface.
Implementar a classe iPhone que implementa todas as interfaces.
Implementar as Classes e Interfaces em Java

Criar as interfaces ReprodutorMusical, AparelhoTelefonico, e NavegadorNaInternet.
Implementar a classe iPhone que implementa essas interfaces.
1. Diagrama UML
Vamos criar o diagrama UML para representar as funcionalidades do iPhone como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

Diagrama UML
plaintext
Copiar código
+-----------------------+
|      ReprodutorMusical|
+-----------------------+
| +tocar(): void        |
| +pausar(): void       |
| +selecionarMusica(musica: String): void |
+-----------------------+

+-----------------------+
|     AparelhoTelefonico|
+-----------------------+
| +ligar(numero: String): void  |
| +atender(): void       |
| +iniciarCorreioVoz(): void |
+-----------------------+

+-----------------------+
|   NavegadorNaInternet |
+-----------------------+
| +exibirPagina(url: String): void |
| +adicionarNovaAba(): void        |
| +atualizarPagina(): void         |
+-----------------------+

+-----------------------+
|        iPhone         |
+-----------------------+
| +tocar(): void        |
| +pausar(): void       |
| +selecionarMusica(musica: String): void |
| +ligar(numero: String): void  |
| +atender(): void       |
| +iniciarCorreioVoz(): void |
| +exibirPagina(url: String): void |
| +adicionarNovaAba(): void |
| +atualizarPagina(): void  |
+-----------------------+
2. Implementação em Java
Interface ReprodutorMusical
java
Copiar código
public interface ReprodutorMusical {
    void tocar();
    void pausar();
    void selecionarMusica(String musica);
}
Interface AparelhoTelefonico
java
Copiar código
public interface AparelhoTelefonico {
    void ligar(String numero);
    void atender();
    void iniciarCorreioVoz();
}
Interface NavegadorNaInternet
public interface NavegadorNaInternet {
    void exibirPagina(String url);
    void adicionarNovaAba();
    void atualizarPagina();
}
Classe iPhone
public class iPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorNaInternet {

    @Override
    public void tocar() {
        System.out.println("Reproduzindo música.");
    }

    @Override
    public void pausar() {
        System.out.println("Música pausada.");
    }

    @Override
    public void selecionarMusica(String musica) {
        System.out.println("Selecionando a música: " + musica);
    }

    @Override
    public void ligar(String numero) {
        System.out.println("Ligando para " + numero);
    }

    @Override
    public void atender() {
        System.out.println("Atendendo a chamada.");
    }

    @Override
    public void iniciarCorreioVoz() {
        System.out.println("Iniciando correio de voz.");
    }

    @Override
    public void exibirPagina(String url) {
        System.out.println("Exibindo página: " + url);
    }

    @Override
    public void adicionarNovaAba() {
        System.out.println("Adicionando nova aba.");
    }

    @Override
    public void atualizarPagina() {
        System.out.println("Atualizando página.");
    }

    public static void main(String[] args) {
        iPhone meuIPhone = new iPhone();
        
        // Testando funcionalidades de reprodutor musical
        meuIPhone.tocar();
        meuIPhone.selecionarMusica("Imagine - John Lennon");
        meuIPhone.pausar();
        
        // Testando funcionalidades de aparelho telefônico
        meuIPhone.ligar("123456789");
        meuIPhone.atender();
        meuIPhone.iniciarCorreioVoz();
        
        // Testando funcionalidades de navegador na internet
        meuIPhone.exibirPagina("https://www.example.com");
        meuIPhone.adicionarNovaAba();
        meuIPhone.atualizarPagina();
    }
}
Explicação do Código
Interfaces: As interfaces ReprodutorMusical, AparelhoTelefonico, e NavegadorNaInternet definem os métodos que representam as funcionalidades do iPhone.
Classe iPhone: A classe iPhone implementa todas as interfaces, fornecendo as implementações dos métodos definidos em cada uma das interfaces.
Main: A função main é usada para testar as funcionalidades da classe iPhone.
