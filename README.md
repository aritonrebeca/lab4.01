public class prob1 {
    public static void main(String[] args) {
        afisareCaractereMijloc("openai");
        afisareCaractereMijloc("java");
        afisareCaractereMijloc("programming");
    }

    public static void afisareCaractereMijloc(String cuvant) {
        int lungime = cuvant.length();
        int mijloc = lungime / 2;

        System.out.print("Cuvântul '" + cuvant + "' - Caracter(e) din mijloc: ");
        if (lungime % 2 == 0) {
            // Cuvântul are număr par de litere
            System.out.println(cuvant.substring(mijloc - 1, mijloc + 1));
        } else {
            // Cuvântul are număr impar de litere
            System.out.println(cuvant.charAt(mijloc));
        }
    }
}
