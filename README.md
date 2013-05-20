public abstract class Animal {
  private int age;
	private int weight;
	private int speed;
	private int acceleration;
	public void name() {
		System.out.println("Don't have a name yet");
	}

	public void talk() {
		System.out.println("Hello");
	}
//four argument constructor
	public Animal(int weight, int age, int speed, int acceleration) {
		super();
		this.weight = weight;
		this.age = age;
		this.speed = speed;
		this.acceleration = acceleration;
	}

	public int getWeight() {
		return weight;
	}
	public void setWeight(int weight) {
		this.weight = weight;
	}

	public int getAge() {
		return age;
	}
	public void setAge(int age) {
		this.age = age;
	}
	public int getAcceleration() {
		return acceleration;
	}
	public void setAcceleration(int acceleration){
		this.acceleration = acceleration;
	}
	public int acceleration(int acceleration){
		int A = 0;
		A = acceleration;
		return (0 + (int) (Math.random() * A ));
		
	}

	public int getSpeed() {
		return speed;
	}

	public void setSpeed(int speed) {
		this.speed = speed;
	}

	public static int walk(int speed) {
		int s = 0;
		s = speed;
		return (0 + (int) (Math.random() * s));
	}
	public class Gorilla extends Animal {
  public Gorilla(int weight, int age, int speed, int acceleration) {
		super(age, weight, speed, acceleration);
	}

	public void name() {
		System.out.println("Donkey Kong");
	}

	public void talk() {
		System.out.println("Whoa Whoa");
	}

	public static int walk(int speed) {
		int s;
		s = speed;
		return (0 + (int) (Math.random() * s));
	}
	
}

}
public class Human extends Animal {

  public Human(int weight, int age, int speed, int acceleration) {
		super(age, weight, speed, acceleration);
	}

	public void name() {
		System.out.println("Peter");
	}

	public void talk() {
		System.out.println("Hello My name is Peter");
	}

	public static int walk(int speed) {
		int m;
		m = speed;
		return 0 + (int) (Math.random() * m);
	}
	
}
public class Robot extends Animal {
  public Robot(int weight, int age, int speed, int acceleration) {
		super(age, weight, speed, acceleration);
	}

	public void name() {
		System.out.println("Metroid");
	}

	public void talk() {
		System.out
				.println("He - e-e ll -o-o My na--me is Me-e-e tro-o-o-o i-i-i-i d-d-d");
	}

	public static int walk(int speed) {
		int k;
		k = speed;
		return 0 + (int) (Math.random() * k);
	}
}


public class Testprogram {
  public static void main(String args[]) {
		Gorilla object = new Gorilla(5, 500, 40, 10);
		Human object1 = new Human(21, 150, 25, 5);
		Robot object2 = new Robot(3, 1000, 100, 20);
		// Gorilla
		object.name();
		object.talk();
		System.out.println("Gorilla weight:" + object.getWeight() + "lbs"
				+ "\nGorilla age:" + object.getAge() + " Years"
				+ "\nGorilla speed:" + object.getSpeed() + " mph"
				+ "\nGorilla acceleration:" + object.getAcceleration() + "ft/s");

		// Human
		object1.name();
		object1.talk();
		System.out.println("Human weight:" + object1.getWeight() + "lbs"
				+ "\nHuman age:" + object1.getAge() + "Years"
				+ "\nHuman speed:" + object1.getSpeed() + " mph"
				+ "\nHuman acceleration:" + object1.getAcceleration()+ "ft/s");

		// Robot
		object2.name();
		object2.talk();
		System.out.println("Robot weight:" + object2.getWeight() + "lbs"
				+ "\nRobot age:" + object2.getAge() + "Years"
				+ "\nRobot speed:" + object2.getSpeed() + " mph"
				+ "\nRobot acceleration:" + object2.getAcceleration() + "ft/s");
	}
}



