# sw JAR decompiler

This is a product containing a decompiler that will create Magik code from the jar files that where created from Magik.
The core component is the **decompiler**, contained in the **deco** package.

The basic methods are:
 - decompile a product to a directory
e.g.: *deco:decompiler.new().decompile_product(smallworld_product.products[:sw_core], "c:\temp")*  
 - decompile a product inside the product directory
 e.g.: *deco:decompiler.new().decompile_product(smallworld_product.products[:sw_core])*
 - decompile a single jar to a directory
 e.g.: *deco:decompiler.new().decompile_jar_to_dir("D:\SW5\core\core.jar", "c:\temp")*
 - decompile many jars to a directory
 e.g.: *deco:decompiler.new().decompile_jar_dir_to_dir("D:\SW5\core", ""*.jar, "c:\temp")* 


## create the decompiler
The **new()** method for de decompiler takes two optional arguments:
 - p_safe?: continue the decompilation even when an error occurs. Default = _true.
 - p_overwrite?: overwrite any existing magik files. Default = _false.

