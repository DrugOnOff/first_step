
public class first {

	/**
	* @param args
	*/
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		String name="oleg"; 
		String alpha=" abcdefghiklmnopqrstvxyz";
		
		int leter=0,sumNumbersOfName=0;
		while (leter<name.length()) {
		char let = name.charAt(leter);
		int numberOfLeter=alpha.indexOf(let);
		leter++;
		sumNumbersOfName+=numberOfLeter;
		}
	
	
		if (sum(sumNumbersOfName) < 10) 
		System.out.println(sum(sumNumbersOfName));
		else 
		while (sum(sumNumbersOfName)>=10){
			sumNumbersOfName=sum(sumNumbersOfName);
			System.out.println(sum(sumNumbersOfName));	
		}
				
	}


	public static int sum (int last) {
		int tempResult = 0;
		while (last>=10) {
		int result =last%10;
		last=last/10;
		tempResult+=result;
		}
//		last=tempResult+last;
		return tempResult+last;
		}
	}


