// Online Java Compiler
// Use this editor to write, compile and run your Java code online
class Main {
    public static void main(String[] args) {
        int arr[] = { 900, 940, 950, 1100, 1500, 1800};
        int dep[] = { 910, 1200, 1120, 1130, 1900, 2000};
        int platform =0, max=1,q=0,r=0;
        while(r < dep.length ){
            if(arr[q]<dep[r] && q < arr.length -1){
                platform ++;
                q++;
            }
            else{
                r++;
                if(platform>max)
                    max=platform;
                platform--;
            }
        }
        System.out.println("Number of platform required is: "+max);
    }
}

// Output: Number of platform required is: 3
    
