# OOP4-INHERITANCE

#KODE UNTUK MAHASISWA
public class mahasiswa extends person {
    int nim;
    String jurusan;

    public void setNim(int nim){
        this.nim= nim;  
    
    }

    public void setJurusan(String jurusan){
        this.jurusan = jurusan;
    }
     public int getNim(){
        return this.nim;
     }

    public String getJurusan(){
        return this.jurusan;
    }

     public void cetakmahasiswa() {
        System.out.println("Nama : " + getNama());
        System.out.println("Jenis Kelamin : " + getJeniskelamin());
        System.out.println("Umur : " + getUmur());
        System.out.println("Alamat : " + getAlamat());
        System.out.println("Jurusan :" + getJurusan());
        System.out.println("Nim :" + getNim());
    }
    public static void main(String[] args) {
        mahasiswa anton = new mahasiswa();
        mahasiswa riko = new mahasiswa();
         
         anton.setNama("Anton Lari Maraton");
        anton.setJeniskelamin("Laki-laki");
        anton.setUmur(99);
        anton.setAlamat("Perum GPI CUYY");
        anton.setNim(909090);
        anton.setJurusan("Informatika");

        riko.setNama("Riko Cox");
        riko.setJeniskelamin("Perempuan");
        riko.setUmur(1);
        riko.setAlamat("Perum KURANG KURANG DALAM PERAHU");
        riko.setNim(10101010);
        riko.setJurusan("Nganggur");

        System.out.println("Info Anton:");
        anton.cetakmahasiswa();
        System.out.println("\nInfo Riko:");
        riko.cetakmahasiswa();
        
    }

}
