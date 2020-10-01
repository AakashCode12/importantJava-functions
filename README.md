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

### Inserting a character in a String

      public static String insertCharacterInBetween(String str, char cr, int index) {
            /*  !here the str is original String,
                !cr is the character to be inserted and
                !index is the index at which we need to insert the character
            */
            str = str.substring(0, index) + cr + str.substring(index + 1);// modified string
            return str;
        }

### Sort a String function in java

    public static String sortAlphabeticallyString(String str) {
            char charArray[] = str.toCharArray();
            Arrays.sort(charArray);
            return new String(charArray);
        }

### to Sort a string or alphabet if we have its position in array

##### If we have something like arr[]={0,3,1} & str[]={"a","d","b"} as input. & we want to sort the alphabetical order stored in string.

##### Then we can sort it using this code. We can't use the Arrays.sort(charArray); in some cases when we also need the indexes in the array.

##### here we have arr[] with all the indexes and str[] with all the strings..

     int temp = 0;
     String tempstr = "";
     for (int i = 0; i < n - 1; i++) {
                for (int j = i + 1; j < n; j++) {
                    if (arr[j] < arr[i]) {
                        temp = arr[i];
                        arr[i] = arr[j];
                        arr[j] = temp;

                    tempstr = str[i];
                    str[i] = str[j];
                    str[j] = tempstr;

                }
            }
        }
