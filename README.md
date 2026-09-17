Lab1-Task1 
Create two directories and move all files instead of copying from one directory to another
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> mkdir dir1


    Directory: C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        17.09.2026     13:13                dir1


PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> mkdir dir2


    Directory: C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        17.09.2026     13:13                dir2


PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> cd .\dir1\
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1> New-Item my_file.txt


    Directory: C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        17.09.2026     13:17              0 my_file.txt


PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1> New_Item my_file2.txt
New_Item : The term 'New_Item' is not recognized as the name of a cmdlet, function, script file, or operable program. C
heck the spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:1
+ New_Item my_file2.txt
+ ~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (New_Item:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1> New-Item my_file2.txt


    Directory: C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        17.09.2026     13:18              0 my_file2.txt


PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1> cd..
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> mv /dir1* /dir2
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> cd dir2
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir2> ls
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir2> ls
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir2> cd..
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> cd .\dir1\
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1> ls


    Directory: C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        17.09.2026     13:17              0 my_file.txt
-a----        17.09.2026     13:18              0 my_file2.txt


PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir1> cd ..
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> mv dir1\* dir2\
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1> cd .\dir2\
PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir2> ls


    Directory: C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir2


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        17.09.2026     13:17              0 my_file.txt
-a----        17.09.2026     13:18              0 my_file2.txt


PS C:\Users\bakirov_maksat\OneDrive\Desktop\informatio_securitylab1\dir2>
