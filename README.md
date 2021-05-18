# Job Scheduling

# 그리디알고리즘

 ## 알고리즘
 
 
        JobScheduling
        
        
          입력: n개의 작업 t1, t2, ... , tn
          출력: 각 기계에 배정된 작업 순서
          시작시간의 오름차순으로 정렬한 작업 리스트를 L이라고 한다.
          while (L ≠ ∅) {
            L에서 가장 이른 시작시간을 가진 작업 ti를 가져온다.
            if (ti를 수행할 기계가 있으면)
              ti를 수행할 수 있는 기계에 배정한다.
            else
              새로운 기계에 ti를 배정한다.
            ti를 L에서 제거한다.
          }
          return 각 기계에 배정된 작업 순서
          
### 입력
: [s,f]에서 s는 시작시간, f는 종료시간.

t1 = [7,8],

t2 = [3,7],

t3 = [1,5],

t4 = [5,9],

t5 = [0,2],

t6 = [6,8],

t7 = [1,6]

![ㅋㅇㅋ12_210518_161209](https://user-images.githubusercontent.com/80369805/118608183-5e7bb180-b7f4-11eb-89a0-057b905b36d0.jpg)



### 시간복잡도

: n개의 작업을 정렬하는데 O(nlogn)시간이 걸리고,

반복문에서 작업을 가져다 수행가능한 기계에 배정하므로 O(m)의 시간이 걸린다.

루프는 총 n번 수행되므로  O(m)* n=O(mn),  따라서

O(nlogn)+O(nm) 의 시간이 걸린다.


