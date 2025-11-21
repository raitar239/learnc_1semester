**ЛАБОРАТОРНАЯ РАБОТА 9**
GIT
-
---
#### На 3
1. Используем git status:
    ```
    On branch main
    Your branch is up to date with 'origin/main'.
    ```

2. Используем git log:
    ```
    commit 8c4c3caef4939cb1651a63cf5f913e7eb41cbbbb (HEAD -> main, origin/main, origin/HEAD)
    Author: Raitar <raitar239@gmail.com>
    Date:   Mon Sep 22 00:09:11 2025 +0700

    Correct error
    ```
3. Создаем [файл](sort.c) с quick сортировкой.
   
4. Используем git status:
   ```
    Untracked files:
    (use "git add <file>..." to include in what will be committed)
            ./
   ```

5. Добавляем sort.c в область stage:   `git add sort.c`
   
6. Используем git status: 
   ```
    Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
        new file: sort.c
   ```

7. Коммитим файл: `git commit -m "Create sort.c"`

8. Используем git status (*не отслеживаю readme*): 
   ```
    Untracked files:
    (use "git add <file>..." to include in what will be committed)
            README.md   
    ```

9.  Добавляем комментарий в файл: `// Quick sort numbers`

10. Используем git status: 
    ```
    Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
            modified:   sort.c
    ```

11. Добавляем файл: `git add sort.c`

12. Используем git status: 
    ```
    Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
            modified:   sort.c   
    ```

13. Меняем комментарий: `// Quick sort`
    
14. Коммитим: `git commit`
    
15. git status:
    ```
    Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
            modified:   sort.c
    ```
    git log:
    ```
    commit a370e82b495815d6dba3b6d4e329574a88f0abc6 (HEAD -> main, origin/main, origin/HEAD)
    Author: Raitar <raitar239@gmail.com>
    Date:   Fri Nov 21 12:43:42 2025 +0700
        Change comm
    ```

16. Добавляем в stage и коммитим:
     ```
    git add sort.c
    git commit -m "Change comment"
     ```
    
17. Пушим на githab (*пушил каждый commit*): `git push`