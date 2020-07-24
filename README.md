![The Trouble with TypeScript - DEV](https://res.cloudinary.com/practicaldev/image/fetch/s--Rx2-HaVZ--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/bq5nm2vl3thxju1l5y24.png)

1. TypeScript를 빠르게 배워봅시다.
2. 6월25일까지 다 완료하고 Master 합니다.
3. Hack!

## 1. What is TypeScript?

TypeScript는 새로운 언어가 아닌 JavaScript에서 새,로운 기능이 추가된 언어입니다. 브라우저는 TypeScript를 읽을 수 없으므로 JavaScript로 변환한뒤 실행하게 됩니다.

## 2.  Why TypeSCript?

한가지 예를 들어봅시다.

* JavaScript

  ```javascript
  function add(num1, num2) {
  	return num1 + num2;
  }
  
  console.log(add('2','3'));
  ```

  이 코드는 오류를 발생하지 않지만 예상된 결과가 나오지 않습니다. 2 더하기 3은 5라고 예상할 수 있지만, JavaScript에서는 변수에 타입을 할당하지 않으므로 String으로 계산하게 됩니다. 따라서 5가 아닌 23이란 엉뚱한 값을 얻게 됩니다.

  이런 문제를 해결하기 위해서 TypeScript를 사용합니다.

## 3. TypeScript 사용하기

* 설치하기

  npm으로 설치하면 됩니다.

  ```bash
  npm install -g typescript
  ```

* JavaScript로 컴파일하기

  ```typescript
  const button = document.querySelector('button');
  const input1 = document.getElementById('num1')! as HTMLInputElement;
  const input2 = document.getElementById('num2')! as HTMLInputElement;
  
  function add(num1: number, num2: number) {
    return num1 + num2;
  }
  
  button.addEventListener('click', function () {
    console.log(add(+input1.value, +input2.value));
  });
  
  ```

  위와 같은 파일이 있다고 합시다. 이 파일을 JavaScript로 변경하기 위해서는

  ```bash
  tsc using-ts.ts
  ```

  라는 커맨드를 만들면 javascript로 변경되게 됩니다.

  ```javascript
  var button = document.querySelector('button');
  var input1 = document.getElementById('num1');
  var input2 = document.getElementById('num2');
  function add(num1, num2) {
      return num1 + num2;
  }
  button.addEventListener('click', function () {
      console.log(add(+input1.value, +input2.value));
  });
  
  ```

## 4. TypeScipt Overview

* TypeScript는 기본적으로 Type을 지정해줘야 합니다.
* 브라우저가 이해할 수 있도록 JavaScript로 변환해줘야 합니다.
* JavaScript에는 없는 인터페이스와 사용할 변수의 타입을 미리 지정하는 Generics 기능이 있습니다.
* Decorators 같은 메타 프로그래밍 기능이 있습니다.
* TypeScript는 작성한 코드를 확인하기 쉽습니다.
* Visual Studio Code 같은 IDE를 사용하면 더 쉽게 코드를 작성할 수 있습니다.

# 5. 목차

1. TypeScript 기본
   * 컴파일러와 환경설정
   * Next-gen JS Code
   * Classes & Interfaces
2. Types 과 TypeSrcipt 기능
   * Generics
   * Decorators
   * 프로젝트에 적용하기
3. Namespaces & Modules 사용하기
   * Webpack & TypeScript
   * Third-Party Libraries & TypeScript
   * React+ TypeScript & NodeJS + TypeScript


## 우리팀에서 안쓴다. 잠정 중단

























