# FilmeAn-nimo
public class Ficha {
    String Titulo;
    String Artista;
    int AnoDeLnaçamento;
    double somaDasAvaliacoes;
    int totalDeAvaliacoes;

    void exibeFichaTecnica() {
        System.out.println("Nome do filme: " + Titulo);
        System.out.println("Ano de lançamento: " + Artista);
        System.out.println("Duração em minutos: " + AnoDeLnaçamento);
    }

    void avalia(double nota) {
        somaDasAvaliacoes += nota;
        totalDeAvaliacoes++;
    }

    double pegaMedia() {
        return somaDasAvaliacoes / totalDeAvaliacoes;
    }
}
public class musica {
    public static void main(String[] args) {
        Ficha pessoal = new Ficha();

        pessoal.Titulo = "Anônimo";
        pessoal.Artista = "Bob Odenkirk";
        pessoal.AnoDeLnaçamento = 2021;

        pessoal.exibeFichaTecnica();
        pessoal.avalia(9);
        pessoal.avalia(10);
        pessoal.avalia(9);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(9);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);

        System.out.println("Média de avaliações do filme: " + pessoal.pegaMedia());
    }
}
// saida Nome do filme: Anônimo
// Ano de lançamento: Bob Odenkirk
// Duração em minutos: 2021
// Média de avaliações do filme: 9.75
 
