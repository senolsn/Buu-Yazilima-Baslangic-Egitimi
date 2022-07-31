# Insertion Sort Project



Proje 1
[22,27,16,2,18,6] -> Insertion Sort

1-Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
Answer- Step1 [16|27,22,2,18,6]
        Step2 [16,22|27,2,18,6]
        Step3 [2,16,22|27,18,6]
        Step4 [2,6,16,22|18,27]
        Step5 [2,6,16,18,22|27]

2-Big'O gösterimini yazınız.
Answer- n+(n-1)+(n-2)+...+1 = [n(n+1)]/2 => O(n^2)

3-Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
Answer- Average case; O(n^2) , Worst case O(n^2) , Best case; O(n)

4-Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
Answer- [2,6,16,18,22,27] sorted array; 18 in the middle of the array so we indentify it as average case.

5-[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
Answer- Step1 [3|7,5,8,2,9,4,15,6]
        Step2 [3,5|7,8,2,9,4,15,6]
        Step3 [2,3,5|8,7,9,4,15,6]
        Step4 [2,3,5,7|8,9,4,15,6]
        
    
# Merge Sort Project


[16,21,11,8,12,22] -> Merge Sort

1-Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Answer- Step1-     [16,21,11]     |      [8,12,22]
        Step2- [16,21]  |  [11]   |   [8,12]  |  [22]
        Step3- [16] | [21] | [11] | [8] | [12] | [22]
        Step4- [16,21] | [11]     | [8,12]     | [22]
        Step5- [11,16,21]         | [8,12,22]
        Step6-           [8,11,12,16,21,22]

2-Big-O gösterimini yazınız.
Answer- Her parçalayışımızda yarıya bölüyoruz (logn) ve bu işlemi her bir eleman için gerçekleştiriyoruz (n)
        logn * n = n.logn =>  O(nlogn) bulunur.
        
        
        
# Binary Search Tree Project

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Answer- 
Step1- root = 7              7

Step2- 5<7(root)             7
                            /
                           5

Step3- 1<7(root)             7
       1<5                  /
                           5
                          /
                         1
                         
Step4- 8>7(root)             7
                            / \
                           5   8
                          /
                         1
                         
Step5- 3<7(root)             7
       3<5                  / \
       3>1                 5   8
                          / 
                         1   
                          \
                           3

Step6- 6<7(root)             7
       6>5                  / \
                           5   8
                          / \
                         1   6
                          \
                           3

Step7- 0<7(root)             7
       0<5                  / \
       0<1                 5   8
                          / \
                         1   6
                       /  \
                      0    3
                      
Step8- 9>7(root)             7
       9>8                  / \
                           5   8
                          / \   \
                         1   6   9
                       /  \
                      0    3
                      
Step9- 4<7(root)             7
       4<5                  / \
       4>1                 5   8
       4>3                / \   \
                         1   6   9
                       /  \
                      0    3
                            \
                             4
                             
 Step10- 2<7(root)           7
       2<5                  / \
       2>1                 5   8
       2<3                / \   \
                         1   6   9
                       /  \
                      0    3
                          / \
                         2   4
