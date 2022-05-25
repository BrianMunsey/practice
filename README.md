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

# Java Stdin and Stdout II

public class Solution {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int i = scan.nextInt();
        Double d = scan.nextDouble();
        String s = scan.nextLine();
        s = scan.nextLine();

        System.out.println("String: " + s);
        System.out.println("Double: " + d);
        System.out.println("Int: " + i);
    }
}

# Java Output Formatting

public class Solution {

    public static void main(String[] args) {
            Scanner sc=new Scanner(System.in);
            System.out.println("================================");
            for(int i=0;i<3;i++)
            {
                String s1=sc.next();
                    while(s1.length()<15){
                        s1+=" ";
                    }
                int x=sc.nextInt();
                String newNum = String.format("%03d", x);
                System.out.println(s1+newNum);
            }
            System.out.println("================================");

    }
}

# Java Loops I

public class Solution {
    public static void main(String[] args) throws IOException {
        BufferedReader bufferedReader = new BufferedReader(new InputStreamReader(System.in));

        int N = Integer.parseInt(bufferedReader.readLine().trim());
        for(int i = 1; i<11; i++){
            System.out.println(N + " x " + i + " = " + N*i);
        }

        bufferedReader.close();
    }
}
