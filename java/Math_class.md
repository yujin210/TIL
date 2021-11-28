## [JAVA] 소수점 n 번째 자리 반올림

- Math.round()

  Math 클래스의 round() 메서드는 __실수__의 __소수점 첫 번째 자리를 반올림__하여 __정수로 리턴__시켜준다.

  이를 활용하여 소수점 n 번째 자리까지 나타내는 것도 가능하다.

  

  ex) 원주율 3.14를 소수점 1 번째 자리까지 나타내는 경우를 예로 들자면, 아래와 같은 방법으로 나타낼 수 있다.

  

  1. 3.14 * 10 = 31.4 // 10을 곱해준다.

  2. Math.round(31.4) // Math.round()를 적용시키면 반올림이 적용되어 31이라는 결과가 나온다.

  3. 31 / 10.0 = 3.1 // 2번의 결과인 31에 원래 곱했던 숫자만큼 다시 나눠준다. 

     

  `System.out.println(Math.round(3.14*10)/10.0);`

  정리하면 위와 같은 코드로 출력할 수 있다.

  

  이때, Math.round(3.14*10)으로 반올림 후에 10.0으로 나눠줘야 한다.

  Math.round((3.14*10)/10.0)과 같이 메서드 안에서 곱하는 값과 나눠주는 값을 동시에 넣어주면 다른 결과가 나오게 된다. 

  

  ```java
  double pi = 3.14159265359;
  
  System.out.println(Math.round(pi)); // 결과 : 3
  System.out.println(Math.round(pi*10)/10.0); // 결과 : 3.1
  System.out.println(Math.round(pi*100)/100.0); // 결과 : 3.14
  
  ```

  

  