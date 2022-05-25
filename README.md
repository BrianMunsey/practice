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

# Java Loops II

class Solution{
    public static void main(String []argh){
        Scanner in = new Scanner(System.in);
        int t=in.nextInt();
        for(int i=0;i<t;i++){
            int a = in.nextInt();
            int b = in.nextInt();
            int n = in.nextInt();
            for (int j = 0; j < n; j++) 
            {
                a += b * (int) Math.pow(2, j);
                System.out.print(a + " ");
            }
            System.out.println();
        }
        in.close();
    }
}

# Java Datatypes

class Solution{
    public static void main(String []argh)
    {



        Scanner sc = new Scanner(System.in);
        int t=sc.nextInt();

        for(int i=0;i<t;i++)
        {

            try
            {
                long x=sc.nextLong();
                System.out.println(x+" can be fitted in:");
                if(x>=-128 && x<=127)System.out.println("* byte");
                if(x>=-Math.pow(2,15) && x<=Math.pow(2,15)-1)System.out.println("* short");
                if(x>=-Math.pow(2,31) && x<=Math.pow(2,31)-1)System.out.println("* int");
                if(x>=-Math.pow(2,63) && x<=Math.pow(2,63)-1)System.out.println("* long");
            }
            catch(Exception e)
            {
                System.out.println(sc.next()+" can't be fitted anywhere.");
            }

        }
    }
}

# Java End-of-file

public class Solution {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int i = 1;
        while(scan.hasNext()){
            System.out.println(i + " " + scan.nextLine());
            i++;
        }
    }
}
