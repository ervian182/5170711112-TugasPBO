# 5170711112-TugasPBO
package manusia;

public class Ervian extends Manusia{//clas ervian mewarisi variabel dan method dari super clas manusia
    void bernafas(){//overriden method
    System.out.println("Bernafas Dengan Paru-Paru");
    }
    protected int umur;//variabel umur dengan access protected
    public Ervian(){
        umur = 20;
    }
    
    protected void Pekerjaan(){//method pekerjaan yang tidak dimiliki oleh super clas ervian 
        System.out.println("Ervian");
        System.out.println("Mahasiswa");
    }
}

package manusia;

public class Manusia {

    public static void main(String[] args) {
        Ervian input = new Ervian();
        input.Pekerjaan();//memangil method pekerjaan yang ada di clas Ervian
        System.out.println ("Umur : "+input.umur);//variabel umur bisa dipanggil karena 1 package
        input.bernafas();//memangil method bernafas yang ada di clas Ervian
    }
    void bernafas(){//overriding method
    System.out.println("Bernafas Dengan Paru-Paru");
    }
}
