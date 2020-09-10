# StringMethodlar
CharAt(index) -> string lere uygulanır. String i karakter array olarak ele alıp, belirtilen index deki karakteri getirir.

 -> Manuel String reverse de kullanılıyor.
	
  
    String source="deneme";
    String reverse = "";
    for(int i = source.length()-1; i >=0; i--){
    
      reverse = reverse + source.charAt(i);
      
    }   
    System.out.println(reverse);
 
 substring(index) -> Stringlere uygulanır. index(dahil) den baslayarak string in son elemanını alır (örneğin arr 0 dan baslıyor index 1 olursa 1 den 3 e kadar elemanları alır), string i baştan keser. Geriye string doner.
 
 	String Str = new String("abc");
	System.out.println(Str.substring(1)); 
	// bc
	
 -> recursive string reverse de kullanılır
Aşağıda ana mantık string 1 kez gönderiliyor(recursive oldugu için) aynı string in 0. elemanı string in basından alıp sonuna ekliyoruz.
	 String input = "AliveisAwesome";
  	//create Method and pass input string as parameter
  	String reversed = reverseString(input);
  	System.out.println("The reversed string is: " + reversed);
	
	 public static String reverseString(String input){
		 if (input.isEmpty()){
			return input;
		 }
  		return reverseString(input.substring(1)) + input.charAt(0);
 	}
