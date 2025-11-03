# tugas-6
import java.util.Scanner;

public class PenjumlahanMatriks {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan jumlah baris matriks: ");
        int baris = input.nextInt();

        System.out.print("Masukkan jumlah kolom matriks: ");
        int kolom = input.nextInt();

        int[][] matriksA = new int[baris][kolom];
        int[][] matriksB = new int[baris][kolom];
        int[][] hasil = new int[baris][kolom];

        // Memasukkan elemen matriks A
        System.out.println("Masukkan elemen matriks A:");
        for (int i = 0; i < baris; i++) {
            for (int j = 0; j < kolom; j++) {
                System.out.print("A[" + i + "][" + j + "]: ");
                matriksA[i][j] = input.nextInt();
            }
        }

        // Memasukkan elemen matriks B
        System.out.println("Masukkan elemen matriks B:");
        for (int i = 0; i < baris; i++) {
            for (int j = 0; j < kolom; j++) {
                System.out.print("B[" + i + "][" + j + "]: ");
                matriksB[i][j] = input.nextInt();
            }
        }

        // Menjumlahkan matriks A dan B
        for (int i = 0; i < baris; i++) {
            for (int j = 0; j < kolom; j++) {
                hasil[i][j] = matriksA[i][j] + matriksB[i][j];
            }
        }

        // Menampilkan hasil penjumlahan
        System.out.println("Hasil penjumlahan matriks A + B:");
        for (int i = 0; i < baris; i++) {
            for (int j = 0; j < kolom; j++) {
                System.out.print(hasil[i][j] + "\t");
            }
            System.out.println();
        }

        input.close();
    }
}Potongan kode ini berfungsi untuk **menjumlahkan dua matriks** berukuran sama.

1. Pengguna memasukkan **jumlah baris dan kolom** matriks.
2. Program membuat tiga matriks: `matriksA`, `matriksB`, dan `hasil`.
3. Pengguna mengisi elemen-elemen matriks A dan B melalui input.
4. Program menjumlahkan setiap elemen yang posisinya sama:
   [
   hasil[i][j] = matriksA[i][j] + matriksB[i][j]
   ]
5. Hasil penjumlahan ditampilkan dalam bentuk matriks di layar.


