# Comp8.Average

public static void main(String[] args) {
        if (args.length == 0) {
            System.out.println("No arguments");
        } else {
            int sum = 0;
            for (String arg : args) {
                sum += Integer.parseInt(arg);
            }
            double average = (double) sum / args.length;
            System.out.println("The average is: " + average);
        }
    }
}
