class Main {
    public static void main(String[] args) {
        int[] a={10,20,30,40,50,60,70};
        int n=33;
        boolean flag=false;
        int l=0;
        int r=a.length-1;
        while(l<=r){
            int m=(l+r)/2;
            if(a[m]==n){
                flag=true;
            }
            else if(a[m]<n){
                l=m+1;
            }
            else if(a[m]>n){
                r=m-1;
            }
        }
        if(flag==true){
            System.out.print("Found");
        }
        else{
            System.out.print("Not Found");
        }
    } 
}   
