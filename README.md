# practice
My Java practice from Hackerrank

# Java Stdin and Stdout I

public class Solution {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int a = scan.nextInt();
        int b = scan.nextInt();
        int c = scan.nextInt();

        System.out.println(a);
        System.out.println(b);
        System.out.println(c);
    }
}

# Java If-Else

public class Solution {



    private static final Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        
        int N = scanner.nextInt();
        scanner.skip("(\r\n|[\n\r\u2028\u2029\u0085])?");
               if(N%2 == 0)
    {
        if(N>=2 && N<=5)
        {
            System.out.println("Not Weird");
        }
        else if(N>=6 && N<=20)
        {
            System.out.println("Weird");
        }
        else
        {
            System.out.println("Not Weird");
        } 
    }
    else
    {
        System.out.println("Weird");
    }
        scanner.close();
    }
}
