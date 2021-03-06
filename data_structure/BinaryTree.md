# **이진 트리**

## 작성자
[![tdm1223](https://avatars1.githubusercontent.com/u/21440957?s=100&v=4)](https://github.com/tdm1223)

## 이진 트리
- 모든 노드가 **2개**의 서브 트리를 가지고 있는 트리
- 서브 트리는 **공집합**일 수 있다.
- **공집합도 이진트리**이다.

## 정의
1. 공집합이거나
2. 루트와 왼쪽 서브 트리, 오른쪽 서브 트리로 구성된 노드들의 유한 집합으로 정의된다.
3. 이진 트리의 서브 트리들은 모두 이진 트리여야 한다.

## 성질
- n개의 노드를 가진 이진 트리는 **n-1개의 간선**을 가진다.
- 높이가 h인 이진트리의 경우, 최소 **h개의 노드**를 가진다.
- 높이가 h인 이진트리의 경우, 최대 **2<sup>h</sup>-1개의 노드**를 가진다.
- 레벨 i에서의 노드의 최대 개수는 **2<sup>i-1</sup>개**이다.

## 분류
1. 포화 이진 트리
    - 트리의 각 레벨에 노드가 꽉 차 있는 이진 트리
2. 완전 이진 트리
    - 높이가 k일 때 레벨 1부터 k-1까지는 모두 채워져 있다.
    - 마지막 레벨 k에서는 왼쪽부터 오른쪽으로 노드가 순서대로 채워져 있다.
3. 기타 이진 트리

## 이진 트리의 표현
1. 배열을 이용
    - 완전 이진트리를 표현할 때
    - 노드 i의 부모 노드 인덱스 = ⌊i/2⌋
    - 노드 i의 왼쪽 자식 노드 인덱스 = 2i
    - 노드 i의 오른쪽 자식 노드 인덱스 = 2i + 1
2. 포인터를 이용
    - 일반적인 이진트리를 표현할 때
    - 노드 클래스나 구조체를 만든다.
    - ```cpp
        class Node{
            int data;
            Node *left;
            Node* right;
        };
        ```

## 참조
- C언어로 쉽게 풀어쓴 자료 구조 개정판. 천인국, 공용해 공저

