import java.util.ArrayList;
public class TestArrayList {

	public static void main(String[] args) {
		//create list to store ints
ArrayList<Integer> TestList = new ArrayList<>();

//this segment prints out the original array
System.out.println("normal list");
int x = 0;
while (x != 11) {
TestList.add(x);
System.out.println(TestList.get(x));
x = x+1;	
}




System.out.println("shuffled list");
int z=0;
while (z != 11) {
// decides which two elements get swapped
	int rand = (int)(Math.random()* 11);
	int rand2 = (int)(Math.random()* 11);
	//holds one of the elements so it doen't get deleted while swapping
	int hold=TestList.get(rand);
//swaps two random elements
	TestList.set(rand, rand2);	
	TestList.set(rand2, hold);

		
	//prints "shuffled" list
System.out.println(TestList.get(z));
z = z+1;	
}
	
	
	
	
	
	
	
	
	
	
	
	}

}
  
