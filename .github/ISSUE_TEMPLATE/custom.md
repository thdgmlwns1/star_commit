---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

**제목:**  
`[BUG] Internet Explorer에서 결제 버튼 작동 안 함`

**문제 요약:**  
Internet Explorer 11에서 결제 페이지의 "결제하기" 버튼이 클릭되지 않는 문제가 발생합니다. 다른 브라우저에서는 정상 작동합니다.

**발생 환경:**  
- 브라우저: Internet Explorer 11 (버전 11.0.9600.19596)  
- 운영체제: Windows 10 Pro  
- 웹 애플리케이션 버전: v1.3.2  
- 서버 환경: AWS EC2 (Nginx 1.21, Node.js 14)

**재현 방법:**  
1. [홈페이지 링크](https://example.com)에 접속.  
2. 상품을 장바구니에 추가.  
3. "결제하기" 버튼 클릭.  
4. 아무런 반응이 없음.

**예상 결과:**  
버튼 클릭 시 결제 프로세스가 시작되어야 함.

**실제 결과:**  
- Internet Explorer에서 버튼 클릭 이벤트가 발생하지 않음.  
- JavaScript 콘솔에 다음 오류 출력:  
  ```javascript
  SCRIPT5009: 'Promise' 정의되지 않음  
  ```

**첨부 파일:**  
![Image](https://github.com/user-attachments/assets/5c564087-58a8-43b0-b7ad-2bd2791bce6a)

**관련 이슈:**  
- #2 "결제 API 개선"

**태그:**  
`bug`, `urgent`, `browser-compatibility`
