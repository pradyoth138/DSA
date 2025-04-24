public class Two_Sum {
	public static int [] Tar (int[] arr,int target) {
		
		for(int i=0;i<arr.length;i++) {
			for(int j=i+1;j<arr.length;j++) {
				if(arr[i]+arr[j]==target) {
					return new int[] {i,j};
				}
			}
		}
		return new int[] {};
		
	}	

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int [] arr= {2,7,11,15};
		int target=9;
		
		int[] result = Tar(arr, target);
        // Print the indices of the two numbers
        if (result.length == 2) {
            System.out.println("Indices: [" + result[0] + ", " + result[1] + "]");
        } else {
            System.out.println("No solution found.");
        }

	}

}
