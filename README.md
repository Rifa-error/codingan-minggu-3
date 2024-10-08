import java.util.Scanner;

public class ganjilgenap2 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("=== Menentukan Bilangan Ganjil Genap === ");
        System.out.print("Masukan sebuah angka: ");
        int angka = input.nextInt();

        if (angka % 2 == 0){
            System.out.println(angka + " adalah bilangan genap. ");
        } else {
            System.out.println(angka + " adalah bilangan ganjil. ");
    }

    input.close();
    }
    
}


import java.util.Scanner;

public class lulustidaklulus {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("=== Menentukan Lulus ===");

        System.out.print("Masukan nilai mahasiswa : ");
        double nilaiMahasiswa = scanner.nextDouble();

        String keterangan;

        if (nilaiMahasiswa >=75) {
            keterangan = "lulus";
        } else{
            keterangan = "Tidak lulus";
        }

        System.out.println("Keterangan : " + keterangan);

        scanner.close();
    }
}



import java.util.Scanner;

public class konversinilai {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("=== Konversi Nilai Menjadi Grade === ");


        double persenAbsen = 10.0/100; 
        double persenTugas = 20.0/100; 
        double persenProject = 25.0/100;  
        double persenQuiz = 5.0/100;  
        double persenUts = 20.0/100;   
        double persenUas = 20.0/100;   

        System.out.print("Masukkan Nama Mahasiswa : ");
        String namaMahasiswa = scanner.nextLine();

        System.out.print("Masukkan nilai absen : ");
        double nilaiAbsen = scanner.nextDouble();

        System.out.print("Masukkan nilai tugas : ");
        double nilaiTugas = scanner.nextDouble();

        System.out.print("Masukkan nilai project : ");
        double nilaiProject = scanner.nextDouble();

        System.out.print("Masukkan nilai quiz : ");
        double nilaiQuiz = scanner.nextDouble();

        System.out.print("Masukkan nilai UTS : ");
        double nilaiUts = scanner.nextDouble();

        System.out.print("Masukkan nilai UAS : ");
        double nilaiUas = scanner.nextDouble();

        double nilaiAkhir = (nilaiAbsen * persenAbsen) +
                            (nilaiTugas * persenTugas) +
                            (nilaiProject * persenProject) +
                            (nilaiQuiz * persenQuiz) +
                            (nilaiUts * persenUts) +
                            (nilaiUas * persenUas);

        String grade;
        String keterangan;

        if (nilaiAkhir >= 85) {
            grade = "A";
        } else if (nilaiAkhir >= 75) {
            grade = "B";
        } else if (nilaiAkhir >= 65) {
            grade = "C";
        } else if (nilaiAkhir >= 55) {
            grade = "D";
        } else {
            grade = "E";
        }

        if (nilaiAkhir >= 85) {
            keterangan = "Lulus";
        } else if (nilaiAkhir >= 75) {
            keterangan = "Lulus";
        } else if (nilaiAkhir >= 65) {
            keterangan = "Remedial";
        } else if (nilaiAkhir >= 55) {
            keterangan = "Tidak lulus";
        } else {
            keterangan = "Tidak lulus";
        }

        System.out.println(" === Kesimpulan === ");

        System.out.println("Nama mahasiswa : " + namaMahasiswa);
        System.out.println("Nilai akhir mahasiswa : " + (int)nilaiAkhir);
        System.out.println("Grade mahasiswa : " + grade);
        System.out.println("Keterangan : " + keterangan);

        scanner.close();
    }
}



import java.util.Scanner;

public class pecahanuang {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("=== Menghitung Pecahan uang === ");

        System.out.print("Masukkan jumlah uang: ");
        int jumlahUang = scanner.nextInt();

        int seratusRibu, limaPuluhRibu, duaPuluhRibu, sepuluhRibu, limaRibu, duaRibu, seribu, limaRatus, seratus;

        if (jumlahUang >= 100000) {
            seratusRibu = jumlahUang / 100000;
            jumlahUang = jumlahUang % 100000;
            System.out.println(seratusRibu + " lembar/keping 100000 rupiah");
        }

        if (jumlahUang >= 50000) {
            limaPuluhRibu = jumlahUang / 50000;
            jumlahUang = jumlahUang % 50000;
            System.out.println(limaPuluhRibu + " lembar/keping 50000 rupiah");
        }

        if (jumlahUang >= 20000) {
            duaPuluhRibu = jumlahUang / 20000;
            jumlahUang = jumlahUang % 20000;
            System.out.println(duaPuluhRibu + " lembar/keping 20000 rupiah");
        }

        if (jumlahUang >= 10000) {
            sepuluhRibu = jumlahUang / 10000;
            jumlahUang = jumlahUang % 10000;
            System.out.println(sepuluhRibu + " lembar/keping 10000 rupiah");
        }

        if (jumlahUang >= 5000) {
            limaRibu = jumlahUang / 5000;
            jumlahUang = jumlahUang % 5000;
            System.out.println(limaRibu + " lembar/keping 5000 rupiah");
        }

        if (jumlahUang >= 2000) {
            duaRibu = jumlahUang / 2000;
            jumlahUang = jumlahUang % 2000;
            System.out.println(duaRibu + " lembar/keping 2000 rupiah");
        }

        if (jumlahUang >= 1000) {
            seribu = jumlahUang / 1000;
            jumlahUang = jumlahUang % 1000;
            System.out.println(seribu + " lembar/keping 1000 rupiah");
        }

        if (jumlahUang >= 500) {
            limaRatus = jumlahUang / 500;
            jumlahUang = jumlahUang % 500;
            System.out.println(limaRatus + " lembar/keping 500 rupiah");
        }

        if (jumlahUang >= 100) {
            seratus = jumlahUang / 100;
            jumlahUang = jumlahUang % 100;
            System.out.println(seratus + " lembar/keping 100 rupiah");
        }

        scanner.close();
    }
}



import java.util.Scanner;

public class hargajeruk {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("=== Menghitung Harga Jeruk === ");

        System.out.print("Masukkan jumlah buah jeruk: ");
        int buah = scanner.nextInt();

        int harga_5 = 10000, harga_2 = 5000, harga_1 = 3000;
        int total = 0;

        if (buah >= 5) {
            int harga_buah_5 = (buah / 5) * harga_5;
            buah = buah % 5; 
            total += harga_buah_5;
        }

        if (buah >= 2) {
            int harga_buah_2 = (buah / 2) * harga_2;
            buah = buah % 2; 
            total += harga_buah_2;
        }

        if (buah >= 1) {
            int harga_buah_1 = buah * harga_1;
            total += harga_buah_1;
        }

        System.out.println("Total harga: " + total);
        scanner.close();
    }
}
