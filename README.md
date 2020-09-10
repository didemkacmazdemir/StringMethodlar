# StringMethodlar
CharAt(index) -> string lere uygulanır. String i karakter array olarak ele alıp, belirtilen index deki karakteri getirir.
 -> Manuel String reverse de kullanılıyor.
	String source="deneme";
  
  String reverse = "";
  
    for(int i = source.length()-1; i >=0; i--){
    
      reverse = reverse + source.charAt(i);
      
    }
    
  System.out.println(reverse);
