# Arrays
Arrays check for coursework00

import java.util.Arrays;

public class ArrayCheck {
	public static void main(String[] args) {

    	int[] firstArray =  { 1, 1, 9, 4, 5, 6 };
		int[] secondArray = { 10, 1, 2, 5, 12 };

		printArray("First array", firstArray);
		printArray("Second array", secondArray);
		
		checkArray("First array", firstArray);
		checkArray("Second array", secondArray);
		
	}

	public static void printArray(String arrayName, int[] array) {
		System.out.println(arrayName + " contains:");
		if (array == null ) {
			System.out.println("Nothing");
		} else {
			System.out.println(Arrays.toString(array));
		}
	}


	public static void checkArray(String name, int[] array) {
		for (int j = 0; j < array.length - 1; j++) {
				for (int k = j + 1; k < array.length; k++) {
					if (k != j && array[k] == array[j]) {
			System.out.println(name + " contains duplicated elements.");
		} 
	  }
    }
  }
}
