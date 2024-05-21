# Projeto de Simulação de Smart TV

Este projeto é uma simulação simples de uma Smart TV em Java. Ele demonstra como ligar e desligar a TV, aumentar e diminuir o volume, e mudar de canal. 

## Estrutura do Projeto

O projeto é composto por duas classes principais:

1. **Usuario**: Classe que contém o método `main` para testar as funcionalidades da Smart TV.
2. **SmartTv**: Classe que representa a Smart TV com métodos para ligar, desligar, ajustar o volume e mudar de canal.

## Funcionalidades

- **Ligar e Desligar a TV**
- **Aumentar e Diminuir o Volume**
- **Mudar de Canal**

## Código

### Classe Usuario

```java
public class Usuario {
    
    public static void main(String[] args) throws Exception {
        
        SmartTv smartTv = new SmartTv();
        System.out.println("TV ligada? " + smartTv.ligada);
        System.out.println("Canal atual: " + smartTv.canal);
        System.out.println("Volume atual: " + smartTv.volume);

        smartTv.ligar();

        System.out.println("TV ligada? " + smartTv.ligada);

        smartTv.aumentarVolume();
        smartTv.aumentarVolume();
        smartTv.aumentarVolume();
        smartTv.aumentarVolume();

        System.out.println("Volume atual: " + smartTv.volume);

        smartTv.mudarCanal(15);

        System.out.println("Canal atual: " + smartTv.canal);

    }
}
```

### Classe SmartTV

```java
public class SmartTv {

    boolean ligada = false;
    int canal = 1;
    int volume = 25;

    public void ligar(){
        ligada = true;
    }   

    public void desligar(){
        ligada = false;
    }

    public void aumentarVolume(){
        volume++;
    }

    public void diminuirVolume(){
        volume--;
    }
    
    public void aumentarCanal(){
        canal++;
    }
    
    public void diminuirCanal(){
        canal--;
    }

    public void mudarCanal(int novoCanal){
        canal = novoCanal;
    }
}
```

## Como Executar no VS Code

1. Certifique-se de ter o [Java JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) instalado.

2. Instale o [Visual Studio Code](https://code.visualstudio.com/) e as extensões necessárias para desenvolvimento em Java, como "Extension Pack for Java".

3. Clone este repositório ou baixe os arquivos `Usuario.java` e `SmartTv.java` para uma pasta local.

4. Abra o Visual Studio Code e a pasta onde os arquivos `.java` estão localizados.

5. No VS Code, abra o terminal integrado. Você pode fazer isso clicando em `Terminal` na barra de menu e selecionando `New Terminal`.

6. Clique em Run.

7. Você deve ver a saída no terminal integrado do VS Code, exibindo o estado da TV, o canal atual e o volume.

## Intuito teórico

Este projeto foi desenvolvido com intuito teórico e para fins de estudo. Ele serve como um exemplo prático de como manipular atributos e métodos de uma classe em Java. Para alterar as funcionalidades da Smart TV, as modificações devem ser feitas diretamente na classe Usuario.

##

*Este README foi gerado com auxílio de uma IA.*
   
