# StringMethodlar
CharAt(index) -> string lere uygulanır. String i karakter array olarak ele alıp, belirtilen index deki karakteri getirir.

 -> Manuel String reverse de kullanılıyor.
	
  
    String source="deneme";
    String reverse = "";
    for(int i = source.length()-1; i >=0; i--){
    
      reverse = reverse + source.charAt(i);
      
    }   
    System.out.println(reverse);
 
 substring(index) -> Stringlere uygulanır. index(dahil) den baslayarak string i baslatıp sonlandırır. Geriye string doner.
 
 	String Str = new String("abc");
	System.out.println(Str.substring(1)); 
	// bc
	
 -> recursive string reverse de kullanılır

	 public static String reverseString(String input){
		 if (input.isEmpty()){
			return input;
		 }
  		return reverseString(input.substring(1)) + input.charAt(0);
 	}
