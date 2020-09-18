# importantJava-functions

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
