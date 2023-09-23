# Array
## 정의

- 작업 큐에 들어간 작업이 가장 처음에 처리되는 작업 스케쥴 (First-In-FirstService)
- 한쪽에서는 `삽입연산`만 발생 가능하고, 다른한쪽에서는 `삭제연산`만 발생 가능한 양쪽이 모두 터진 관
- 한쪽에서는 `삽입연산`
    - 서비스를 받기 위한 기다림
- 다른 한쪽에서는 `삭제연산`
    - 서비스를 받는 중
- 선입선출(First-In-First-Out, FIFO) 및 선착 순 서브(First-Come-First-Service, FCFS) 알고리즘과 함께 사용됨

- 예제

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/cbd0be8e-e058-4534-b3bc-3fba11ee8ee5/Untitled.png)

    - rear : 삽입 지점
    - front : 삭제 지점
    - [A, B, C] 총 3개의 원소를 가지고 있다.

## 큐의 객체 정의

- 큐의 추상자료형
    - 큐 객체 : 0개 이상의 원소를 갖는 유한 순서 리스트
- 큐의 연산

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/2f502913-8975-4ad0-ade4-af3a4b5eac88/Untitled.png)

    - 큐의 삽입(Add_q) 연산

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/43d0c6eb-5829-4c20-94d9-2a641927dfa0/Untitled.png)

    - 큐의 삭제(Delete_q) 연산

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/aeab067c-27bc-491b-b9b2-559a4766365e/Untitled.png)

    - 빈 큐 검사(IsEmpty_q) 연산

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/25bf2505-311a-47be-ad28-4d020a319650/Untitled.png)

    - 큐의 만원 검사(IsFull_q) 연산

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/f9256174-46d5-4109-acba-d165e2c6c5f8/Untitled.png)

- Add/Delete 연산의 실행
    - 예제 정의

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/f74f5202-c101-494e-9a5b-a48c9ce156dc/Untitled.png)

    - 1, 2, 3, 4 연산

  ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/9be9730c-6c17-477b-b30b-af626d1bd473/118fe833-8f06-402c-9000-ffb66a328677/Untitled.png)

    - 5, 6, 7, 8 연산 
    - 5, 6, 7, 8 연산