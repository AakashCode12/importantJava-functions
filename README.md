# Important Java Functions

### Function to check a palindrome string 

    public static boolean palindromeString(String s) {

      StringBuilder sb = new StringBuilder();
      sb.append(s);
      sb.reverse();
      String reversedString = sb.toString();

      if (reversedString.equals(s)) {
          return true;
      } else {
          return false;
      }

    }

### Inserting a character in String

    String str = "aakash";	//Original String
    System.out.println("Initial String--> "+str);
    char cr = "a".charAt(0); // character to replace
    int index = 2;	// Index where replaced
    str = str.substring(0, index) + cr + str.substring(index + 1);// modified string`
    System.out.println("Final String--> "+str);
