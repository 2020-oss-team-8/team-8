# Chapter1  
## 팀원 github hompage  
+ 강다빈  
  + [강다빈 깃 허브 사이트](https://dabin0513.github.io/)  
+ 백남규  
  + [백남규 깃 허브 사이트](https://parkiy76.github.io/opswtp/)  
+ 박예진  
  + [박예진 깃 허브 사이트](https://parkiy76.github.io/opswtp/)  
+ 서준철  
  + [서준철 깃 허브 사이트](https://seojuncheol1.github.io/)  
+ 조은채  
  + [조은채 깃 허브 사이트](https://parkiy76.github.io/opswtp/)  

# Chapter2  
## 컴퓨터 데이터 구조    
# Stack  
>+ FILO: First In Last Out  
>+ push: 새로운 요소 추가  
>+ pop: 가장 최근에 들어오는 것을 지우기    
>+ Stack의 활용 예시  
>  + 후위 표기법 계산  
>  + 수식의 괄호 검사(연산자 우선순위 표현을 위한 괄호 검사)  

![Stack 사진](https://user-images.githubusercontent.com/63287630/86358634-c5f74400-bcaa-11ea-9082-b3984a33a06e.png)  
+ Stack은 데이터의 삽입과 삭제가 한 방향에서만 이루어지는데 삽입과 삭제가 일어나는 위치를 top이라고 합니다.  

# Queue  
>+ FIFO: First In First Out  
>+ Enqueue: 가장 늦게 온 것은 가장 뒤에  
>+ Dequeue: 가장 앞에 있는 것을 가장 먼저 삭제  
>+ Queue의 활용 예시  
>  + 은행 업무  
>  + 콜센터 고객 대기시간  
>  + 프로세스 관리  
>  + 너비 우선 탐색(BFS, Breath-First Search)구현  

![Queue 사진](https://user-images.githubusercontent.com/63287630/86358684-ddcec800-bcaa-11ea-85fb-1e210287c388.png)  
+ 출구를 머리(front)로 정해서 삭제를 수행하고, 입구는 꼬리(rear)로 정해서 삽입을 수행합니다.  
 
# 트리(Tree)
> + 트리는 노드로 이루어진 자료 구조를 말합니다.
>   + 트리는 하나의 루트 노드를 가집니다.
>   + 루트 노드는 0개 이상의 자식 노드를 갖고 있습니다.
>   + 그 자식 노드 또한 0개 이상의 자식노드를 가지고 있고, 이는 반복적으로 정의 됩니다.

![트리](https://user-images.githubusercontent.com/63287630/86360770-d0670d00-bcad-11ea-928b-012c456acd72.png)

# 트리와 관련된 용어
>      + 루트 노드(root node): 부모가 없는 노드로 트리는 하나의 루트 노드만을 가짐
>      + 단말 노드(leaf node): 자식이 없는 노드를 말합니다.
>      + 내부 노드(internal node): 단말노드가 아닌 노드
>      + 간선(edge): 노드를 연결하는 선
>      + 형제(sibling): 같은 부모를 가진 노드
>      + 노드의 사이즈(size): 자신을 포함한 모든 자손 노드의 개수
>      + 노드의 깊이(depth): 루트에서 어떤 노드에 도달하기 위해 거쳐야 하는 간선의 수
>      + 노드의 레벨(level): 트리의 특정 깊이를 가지는 노드의 집합
>      + 노드의 차수(degree): 하위 트리 개수/ 간선수(degree): 각 노드가 지닌 가지의 수
>      + 트리의 차수(degree of tree): 트리의 최대 차수
>      + 트리의 높이(height): 루트 노드에서 가장 깊숙히 있는 노드의 깊이




## 프로그래밍 응용 1
#### 자바란?

1. 완전한 객체지향 언어이며, 객체지향의 특성인 클래스, 상속, 캡슐화, 다형성 등의 개념이 적  용된 언어이다.  

#### 조건문  
- switch-case문
```java
switch(조건식){
	case: 조건1
    	break;
    case: 조건2
    	break;
    default:
```  

- if 문  
```java
if(조건삭){//조건식이 true일 때 아래 실행문 동작
	실행문;
    실행문;
 }
```  

#### 반복문  
- while문 
```java
while(조건식){}
```

- do-while문 
```java
 do {} while(조건식);
```

- for문 
```java
for(초기식; 조건식; 증감식){}
```

#### 예제 코드  
```java
import java.util.Scanner;
 
public class Gugudan 
{
    public static void main(String args[])
    {
        for( ; ; )    // 범위가 벗어났을경우 계속 입력하기위한 무한 반복문 사용        
        {
            System.out.print("1부터 9까지의 임의의 숫자를 입력하세요 : ");
            Scanner sDan = new Scanner(System.in);
            int dan = sDan.nextInt();
            
            if(dan < 10)    // 1 ~ 9까지 범위 일때
            {
                for(int su = 1 ; su < 10 ; su ++)    // 단이 정해지면 계산 및 출력하기위한 반복문
                {
                    System.out.println(dan + " * " + su + " = " + (dan * su) + " ");
                }
                break;    // 계산이 완료되면 STOP!
            }else
            { 
                System.out.println("1부터 9까지 다시 입력해주세요.");
                continue;    // 1 ~ 9 까지 범위안에 없을시 다시 for문 처음으로 돌아가기위해 continue 사용
            }
        }    
    }
}

```
- 구구단을 출력하는 코드


#### 용어정리  
1. 클래스 : 객체를 만들어 내기 위한 틀  
2. 객체 : 클래스를 통해 만들어진 구현물  
3. 메소드 : 특정 작업을 수행하기 위한 명령문의 집합  
4. 생성자 : 객체가 생성될 때 반드시 수행되어햐 하는 기능  

[TOC]

