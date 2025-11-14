# Vetores-e-Produto-Escalar
Programa em java que cria dois vetores com 10 entradas fornecidas pelo usuario e calcula o produto escalar desses vetores

public static void main(String[] args) {
        
        Scanner sc = new Scanner (System.in);
        
        int [] vetorA = new int[10];
        int [] vetorB = new int[10];
        int produtoEscalar = 0;
        
        System.out.println("Digite os 10 valores do vetor A:");
        
        for (int i = 0; i < 10; i++) {
            System.out.print("A[" + i + "] = ");
            vetorA[i] = sc.nextInt();
        }
        
        System.out.println("Digite os 10 valores do vetor B:");
        
        for (int i = 0; i < 10; i++) {
            System.out.print("B[" + i + "] = ");
            vetorB[i] = sc.nextInt();
        }

        for (int i = 0; i < 10; i++) {
            produtoEscalar += vetorA[i] * vetorB[i];
        }

        System.out.println("O produto escalar dos dois vetores é: " + produtoEscalar);
    }
}
