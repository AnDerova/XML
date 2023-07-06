
## Homework Git, part 2

**1. Create a new repository on your personal account and call it XML.**

**2. Clone this repository to create a local copy on your computer.**
```
$ git clone git@github.com:AnDerova/XML.git
```

**3. Create a new file "new.xml" into your local repository.**
```
$ touch new.xml
```

**4. Stage a "new.xml" for commit.**
```
$ git add new.xml
```
**5. Commit a file that you've staged.**
```
$ git commit -m 'Create new.xml'
```
**6. Push a file in your remote repository on GitHub.**
```
$ git push -u origin main
```
**7. Edit a "new.xml", to add information about yourself (name, age, number of pets, desired salary).**
```
$ vim new.xml

$ cat new.xml
<personalInfo>
<firstName>Anastasiia</firstName>
<lastName>Derova</lastName>
<age>38</age>
<pets>0</pets>
<salary>10000</salary>
</personalInfo>
```
**8. Push the changes in your remote repository to GitHub.com.**
```
$ git commit -a -m 'Add info about person into new.xml' && git push
```
**9. Create a new file "preferences.xml" into your local repository.**
```
$ touch preferences.xml
```
**10. Edit a "preferences.xml", to add information about your preferences (favorite movie, TV shows, food, season, country you'd like to visit).**
```
$ cat preferences.xml
<personalPreferences>
        <favoriteMovie>Forrest Gump</favoriteMovie>
        <favoriteTVshows>Rick and Morty</favoriteTVshows>
        <favoriteFood>Mango</favoriteFood>
        <favoriteSeason>Spring</favoriteSeason>
        <country>Iceland</country>
</personalPreferences>
```
**11. Create a new file "sklls.xml" into your local repository, add information about your skills**
```
$ touch skills.xml
$ vim skills.xml
$ cat skills.xml
<skills>
        <1>Terminal</1>
        <2>GitHub</2>
        <3>Postman</3>
        <4>SQL</4>
        <5>DevTools</5>
        <6>Mobile Testing</6>
</skills>
```
**12. Push the modified files in your remote repository to GitHub.com.**
```
$ git add . && git commit -m 'Create preferences.xml and skills.xml' && git push
```
**13. Create a new file "bug_report.xml" directly on GitHub.**

**14. Click Commit changes.**

**15. Edit a file "bug_report.xml" directly on GitHub in your repository, add bug report.** 

**16. Save changes in your remote repository.**

**17. Keep your local repository in sync with your remote repository.**
```
$ git pull

$ ls -la
total 15
drwxr-xr-x 1 AnDer 197121   0 Jul  6 18:44 ./
drwxr-xr-x 1 AnDer 197121   0 Jul  6 17:39 ../
drwxr-xr-x 1 AnDer 197121   0 Jul  6 18:44 .git/
-rw-r--r-- 1 AnDer 197121 804 Jul  6 18:44 bug_report.xml
-rw-r--r-- 1 AnDer 197121 145 Jul  6 18:13 new.xml
-rw-r--r-- 1 AnDer 197121 246 Jul  6 18:20 preferences.xml
-rw-r--r-- 1 AnDer 197121 113 Jul  6 18:25 skills.xml

$ cat bug_report.xml
<bugReport>
        <id>1</id>
        <severity>Major</severity>
        <environment>Win 10 Chrome 107 108 109 110 111 112 113 114</environment>
        <title>The English version of the page 'Privacy Policy' in 'Sign up' form is linked to the link 'Privacy Policy' from any language except EN, DE</title>
        <steps>
                <step1>Navigate to capital.com</step1>
                <step2>Select any language exсept EN, DE</step2>
                <step3>Click button 'Trade'</step3>
                <step4>Click link 'Privacy policy'</step4>
        </steps>
        <ER>The 'Privacy policy' page is opened in selected language</ER>
        <AR>The 'Privacy policy' page is opened in English</AR>
        <attach>Link</attach>
        <comments>Null</comments>
</bugReport>
```
