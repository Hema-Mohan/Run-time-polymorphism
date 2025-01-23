# Run-time-polymorphism
class fruits{
    void displayinfo(){
        System.out.println("I like Fruits.");
    }
}
class mango extends fruits{
    void displayinfo(){
        System.out.println("I like Mango.");
    }
}
class apple extends fruits{
    void displayinfo(){
        System.out.println("I like Apple.");
    }
}
public class RunTimePolymorphism {

    public static void main(String[] args) {
          fruits f1 = new mango();
          f1.displayinfo();
          fruits f2 = new apple();
          f2.displayinfo();
    }  
}

OUTPUT:
I like Mango.
I like Apple.
