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

      public static String insertCharacterInBetween(String str, char cr, int index) {
            // here the str is original String
            //cr is the character to be inserted and 
            //index is the index at which we need to insert the character
            str = str.substring(0, index) + cr + str.substring(index + 1);// modified string
            return str;
        }
